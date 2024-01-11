---
---

## 说明
> 任务列表可以通过dataview语法 也可以通过tasks插件获取

## 所有未完成的任务

> [!col2] ### 展开所有未完成的任务和过滤含有关键字的任务
> ```dataviewjs
> //filter输入要过滤的任务关键字
> let filter =""
> //noflod 输入要排除的文件夹
> let noflod ='!"88-Template"'
> const groups = dv.pages(noflod).filter(p => p.file.folder != "").groupBy(p => p.file.folder.split("/")[0])
> for (let group of groups) {
> let tasks=dv.pages(`"${group.key}"`).where(t => { return t.file.name != "" }).file.tasks.where(t => t.text.includes(filter) && !t.completed)
> if(tasks.length>0)
> dv.header(3, group.key);
> dv.taskList(
>     tasks,1)
> }
> 
> ```

> [!tip]
> 可以通过输入@ 快速输入日期 支持自然语言格式比如
> `@today` 今天
> `@in 3 days`  3天后
> `@3 days ago`  3天前


## 任务收集【tasks】
通过tasks插件示例
> [!flex]
> %% ad 语法格式书写 %%
> > [!caution] 过期的任务
> > 
> > ```tasks
> > not done
> > due before  today
> > path does not include "88-Template"
> > short mode
> > ```
> > 
> 
> > [!check] 今天要完成的任务
> > 
> > ```tasks
> > not done
> > due on  today 
> > path does not include "88-Template"
> > short mode
> > ```

> [!flex]
> %%也可以用callout 格式书写 %%
> > [!CHECK] 3天内要完成的任务
> > ```tasks
> not done 
> due after today
> due before in 3 days 
> path does not include "88-Template"
> short mode
> >```
> 
> 
> 
> > [!todo] 未两周要完成的任务
> > ```tasks
> > not done 
> > due after today
> > due before in two weeks
> > path does not include "88-Template"
> > short mode
> > 
> > ```
> 



## 任务收集【dataview】

> [!flex]
> %% ad 语法格式书写 %%
> > [!caution] 过期的任务
> > 
> > ```dataview
> > task
> > from !"88-Template"
> > where !completed
> > AND  due <= date(today)
> > sort  file.cday asc
> > ```
> > 
> 
> > [!check] 今天要完成的任务
> > 
> > ```dataview
> > task
> > from !"88-Template"
> > where !completed
> > AND due = date(today)
> > sort  file.cday asc
> > ```

> [!flex]
> %%也可以用callout 格式书写 %%
> > [!CHECK] 3天内要完成的任务
> > ```dataview
> task
> where file.path = this.file.path 
> where !completed
> WHERE due > date(today) + dur(1 days)
> WHERE due <= date(today) + dur(3 days)
> sort  file.cday asc
> >```
> 
> 
> 
> > [!todo] 未两周要完成的任务
> > ```dataview
> > task
> > where file.path = this.file.path 
> > where !completed
> > WHERE due > date(today) + dur(1 days)
> > and due <= date(today) + dur(2 weeks)
> > sort  file.cday asc
> > ```
> 

> [!flex]
> > [!todo] 六月任务
> > ```dataview
> > task
> > where file.path = this.file.path 
> > where !completed
> > WHERE due >= date(2022-06-01) 
> > WHERE due <= date(2022-06-31) 
> > sort  file.cday asc
> > ```
> 
> > [!todo] 当月内的本周任务
> > ```dataview
> > task
> > where file.path = this.file.path 
> > where !completed
> > WHERE due.month = date(today).month 
> > AND due.week = date(today).week
> > sort  file.cday asc
> > ```
> 
> > [!todo] 下月任务
> > ```dataview
> > task
> > where file.path = this.file.path 
> > where !completed
> > WHERE due.month = date(today).month + 1 
> > sort  file.cday asc
> > ```


## 任务举例
- [ ] 读两本书 📅 2022-06-21
- [ ] 完成交接工作📅2022-05-18 
- [ ] 整理资料📅2022-05-17 
- [ ] 学习一些课程📅2022-05-30
- [ ] 提交报告 📅 2022-06-01 
- [ ] 测试任务📅2022-07-13
- [ ] 这是一个带自定义字段的任务记录001[start::2022-05-30]
- [ ] 这是一个带自定义字段的任务记录002[start::2022-06-01]
- [ ] 这是一个带自定义字段的任务记录1 (Group1::  第一组) 
- [ ] 这是一个带自定义字段的任务记录2 (Group1::  第一组) 
- [ ] 这是一个任务带标签的内容 #紧急任务
> [!example] dvjs版本查看超期任务
> 
> ```dataviewjs
> function overdue(t) {
>   let dValidate = moment(t.text, 'YYYY-MM-DD', true);
>   let d = moment(t.text, 'YYYY-MM-DD');
>   let containsValidDate = dValidate._pf.unusedTokens.length==0 ;
>   let isOverdue = d.diff(moment()) <= 0;
>   return (containsValidDate && isOverdue);
> }
> 
> dv.taskList(dv.pages("").file.tasks
> 	.where (t => overdue(t))
> 	.where (t => !t.completed))
> 
> ```

## 查询带自定义字段的任务
> [!flex]
> 
> ```dataview
> TASK 
> where file.path = this.file.path  
> WHERE Group1 
> FLATTEN Group1 
> GROUP BY Group1 
> ```
> 
> ```dataview
> TASK
> where file.path = this.file.path  
> WHERE start = date(today)
> 
> 
> ```

### 查询带标签的任务

```dataview
task
WHERE contains(tags, "#紧急任务")
```

## 列表查询和任务查询的语法差异
```dataview
list
WHERE contains(file.tasks.start, date(today))
```

```dataview
list
WHERE contains(file.tasks.tags, "#紧急任务")
```

