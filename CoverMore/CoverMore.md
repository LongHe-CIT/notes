## Sprint APACP-2401
### Tickets

```jira-search
type: TABLE
query: project = APACP AND status in ("In Progress", QA, "Ready for Production", "Ready for QA", "Ready for QA Deployment", "Ready for UAT", "Ready to work") AND Sprint = 2085 ORDER BY key ASC, priority DESC
limit: 50
columns: KEY, SUMMARY, ASSIGNEE, -PRIORITY, -FIX_VERSIONS, STATUS,
account: helong
```
### 240123D-CMAP

```jira-issue
APACP-856
APACP-983
APACP-982

# This is a comment 
```

```jira-issue
APACP-230
https://innate.atlassian.net/browse/APACP-976
```

- [x] [APACP-856](https://innate.atlassian.net/browse/APACP-856)  
- [x] [APACP-983](https://innate.atlassian.net/browse/APACP-983)
- [x] [APACP-982](https://innate.atlassian.net/browse/APACP-982)

- [ ] [APACP-230](https://innate.atlassian.net/browse/APACP-230)
- [ ] [APACP-976](https://innate.atlassian.net/browse/APACP-976)

see password
```shell
./devops/scripts/drush.sh @cgu.01dev cget shield.settings
```


> [!Paypal 配置] 
> 
> 1.登录到站点上去（ssh）以BUPA举例 
> `./devops/scripts/drush.sh @bupa.01dev ssh`  
> 2.跳到站点目录 
> `cd /mnt/gfs/innateacsf.01dev`  
> 3.打开secret文件把信息添加上去（这个文件对应本地docroot/sites/shared-local.settings.php） 
> `vim secrets.settings.php`

PANDA-AU 

| site | link |
| :--- | ---- |
| Tmoz | https://travelmoneyoz.dev.insurancebycovermore.com/ |
| RCI | https://royalcaribbean.dev.insurancebycovermore.com/ |
| Queen | https://queenslandcountrybank.dev.insurancebycovermore.com |
| NZ | https://citest0103nz.dev.insurancebycovermore.com/ |
| EasyTravel | https://easytravelinsurance.dev.insurancebycovermore.com/ |
| Cgu | https://cgu.dev.insurancebycovermore.com/ |
| Cel | https://celebritycruises.dev.insurancebycovermore.com/ |
| Bupa | https://bupa.dev.insurancebytravelinsurancepartners.com/ |
| Bend | https://bendigobank.dev.insurancebycovermore.com/ |
| Travel Associates | https://travelassociates.dev.insurancebycovermore.com/ |
| AU | https://citest0103.dev.insurancebycovermore.com/ |
| Cruiseabout Travel Insurance | https://cruiseabout.insurancebycovermore.com/ |


|  |  |  |  |
| ---- | ---- | ---- | ---- |
| Application | Partner | Region | Site URL |
| CMAP | AMI | NZ | [amitravelinsurance.poweredbycovermore.com](http://amitravelinsurance.poweredbycovermore.com/) |
| auntbetty | AU | [www.auntbetty.covermore.com.au](http://www.auntbetty.covermore.com.au/) |  |
| AusPost | AU | [auspost.poweredbycovermore.com](http://auspost.poweredbycovermore.com/) |  |
| Bankwest WL | AU | [bankwest.poweredbycovermore.com](http://bankwest.poweredbycovermore.com/) |  |
| ByojetAU | AU | [byojetau.poweredbycovermore.com](http://byojetau.poweredbycovermore.com/) |  |
| celebritycruises | AU | [celebritycruises.insurancebycovermore.com](http://celebritycruises.insurancebycovermore.com/) |  |
| VirginAU | AU | [covermore.virginaustralia.com](http://covermore.virginaustralia.com/) |  |
| FMG | NZ | [fmg-travelinsurance.poweredbycovermore.com](http://fmg-travelinsurance.poweredbycovermore.com/) |  |
| HIF | AU | [hiftravel.poweredbycovermore.com](http://hiftravel.poweredbycovermore.com/) |  |
| AirNZNZ | NZ | [airnznz.poweredbycovermore.com](http://airnznz.poweredbycovermore.com/) |  |
| Air NZ AU | AU | [insurance.airnewzealand.com.au](http://insurance.airnewzealand.com.au/) |  |
| FCNZ | NZ | [insurance.flightcentre.co.nz](http://insurance.flightcentre.co.nz/) |  |
| FCAU | AU | [insurance.flightcentre.com.au](http://insurance.flightcentre.com.au/) |  |
| WebjetNZ | NZ | [webjetnz.poweredbycovermore.com](http://webjetnz.poweredbycovermore.com/) |  |
| WebjetAU | AU | [insurance.webjet.com.au](http://insurance.webjet.com.au/) |  |
| royalcaribbean | AU | [royalcaribbean.insurancebycovermore.com](http://royalcaribbean.insurancebycovermore.com/) |  |
| EasyTravel | AU | [secure.easytravelinsurance.com.au](http://secure.easytravelinsurance.com.au/) |  |
| IAG | NZ | [statetravelinsurance.poweredbycovermore.com](http://statetravelinsurance.poweredbycovermore.com/) |  |
| AHM | AU | [travel.ahm.com.au](http://travel.ahm.com.au/) |  |
| BudgetDirect | AU | [travel.budgetdirect.com.au](http://travel.budgetdirect.com.au/) |  |
| Kogan | AU | [travel.koganinsurance.com.au](http://travel.koganinsurance.com.au/) |  |
| Medibank | AU | [travel.medibank.com.au](http://travel.medibank.com.au/) |  |
| NRMA | AU | [travelinsurance.nrma.com.au](http://travelinsurance.nrma.com.au/) |  |
| VirginNZ | NZ | [virginaustralia.covermore.co.nz](http://virginaustralia.covermore.co.nz/) |  |
| CGU | AU | [cgu.insurancebycovermore.com](http://cgu.insurancebycovermore.com/) |  |
| Bendigo Bank | AU | [bendigobank.insurancebycovermore.com](http://bendigobank.insurancebycovermore.com/) |  |
| Queensland Country Bank | AU | [queenslandcountrybank.insurancebycovermore.com](https://queenslandcountrybank.insurancebycovermore.com/) |  |
| TOMz | AU | [travelmoneyoz.insurancebycovermore.com/](http://travelmoneyoz.insurancebycovermore.com/) |  |
| OZCruising | AU | [ozcruising.insurancebycovermore.com](http://ozcruising.insurancebycovermore.com/) |  |
| Olive Tree Travel | AU | [olivetreetravel.insurancebycovermore.com](http://olivetreetravel.insurancebycovermore.com) |  |
| Travelinsure | AU | [travelinsure.insurancebycovermore.com](http://travelinsure.insurancebycovermore.com) |  |
| World Expeditions | AU | [worldexpeditions.insurancebycovermore.com](http://worldexpeditions.insurancebycovermore.com) |  |
| Live The Dream Travel | AU | [livethedreamtravel.insurancebycovermore.com](http://livethedreamtravel.insurancebycovermore.com) |  |
| iLuv2Travel & Cruise | AU | [iluv2travel.insurancebycovermore.com](http://iluv2travel.insurancebycovermore.com/) |  |
| My Holiday Travel Insurance | AU | [myholidaycentre.insurancebycovermore.com](http://myholidaycentre.insurancebycovermore.com) |  |
| My Cruises Travel Insurance | AU | [mycruises.insurancebycovermore.com](http://mycruises.insurancebycovermore.com) |  |
| Acland Travel | AU | [aclandtravel.insurancebycovermore.com](http://aclandtravel.insurancebycovermore.com) |  |
| National Travel | AU | [nationaltravel.insurancebycovermore.com](http://nationaltravel.insurancebycovermore.com) |  |
| Travel Associates | AU | [travelassociates.insurancebycovermore.com](http://travelassociates.insurancebycovermore.com) |  |
| Travlr Travel Insurance | AU | [travlr.insurancebycovermore.com](http://travlr.insurancebycovermore.com) |  |
| Wandr Travel Insurance | AU | [wandrtravel.insurancebycovermore.com](http://wandrtravel.insurancebycovermore.com) |  |
| Cruiseabout Travel Insurance | AU | [cruiseabout.insurancebycovermore.com](http://cruiseabout.insurancebycovermore.com/) |  |
| Bupa Travel Insurance | AU | [bupa.insurancebytravelinsurancepartners.com](http://bupa.insurancebytravelinsurancepartners.com/) |  |