## Sprint APACP-2401
### Tickets

```jira-search
type: TABLE
query: project = APACP AND status in ("In Progress", QA, "Ready for Production", "Ready for QA", "Ready for QA Deployment", "Ready for UAT", "Ready to work") AND Sprint = 2085 ORDER BY key ASC, priority DESC
limit: 50
columns: KEY, SUMMARY, ASSIGNEE, -PRIORITY, -FIX_VERSIONS, STATUS,
account: helong
```

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


|  |  |
| ---- | ---- |
| Application | Site URL |
| Bankwest WL | http://bankwest.poweredbycovermore.com/ |
| OZCruising | http://ozcruising.insurancebycovermore.com/ |
| Olive Tree Travel | http://olivetreetravel.insurancebycovermore.com |
| World Expeditions | http://worldexpeditions.insurancebycovermore.com |
| Live The Dream Travel | http://livethedreamtravel.insurancebycovermore.com |
| iLuv2Travel & Cruise | http://iluv2travel.insurancebycovermore.com/ |
| My Holiday Travel Insurance | http://myholidaycentre.insurancebycovermore.com |
| My Cruises Travel Insurance | http://mycruises.insurancebycovermore.com |
| Travelinsure | http://travelinsure.insurancebycovermore.com |
| Acland Travel | http://aclandtravel.insurancebycovermore.com |
| National Travel | http://nationaltravel.insurancebycovermore.com |
| Travel Associates | http://travelassociates.insurancebycovermore.com |
| Travlr Travel Insurance | http://travlr.insurancebycovermore.com |
| Wandr Travel Insurance | http://wandrtravel.insurancebycovermore.com |
| Cruiseabout Travel Insurance | http://cruiseabout.insurancebycovermore.com/ |
| ozcruising | https://ozcruising.dev.insurancebycovermore.com/ |
|  |  |
| TOMz | https://travelmoneyoz.dev.insurancebycovermore.com/ |
| RCI | https://royalcaribbean.dev.insurancebycovermore.com/ |
| Queensland Country Bank | https://queenslandcountrybank.dev.insurancebycovermore.com |
| NZ | https://citest0103nz.dev.insurancebycovermore.com/ |
| EasyTravel | https://easytravelinsurance.dev.insurancebycovermore.com/ |
| Cgu | https://cgu.dev.insurancebycovermore.com/ |
| Cel | https://celebritycruises.dev.insurancebycovermore.com/ |
| Bupa Travel Insurance | https://bupa.dev.insurancebytravelinsurancepartners.com/ |
| Bend | https://bendigobank.dev.insurancebycovermore.com/ |
| Travel Associates | https://travelassociates.dev.insurancebycovermore.com/ |
| AU | https://citest0103.dev.insurancebycovermore.com/ |
| Cruiseabout Travel Insurance | https://cruiseabout.insurancebycovermore.com/ |

### 240123D-CMAP

- [x] [APACP-856](https://innate.atlassian.net/browse/APACP-856)  
- [x] [APACP-983](https://innate.atlassian.net/browse/APACP-983)
- [x] [APACP-982](https://innate.atlassian.net/browse/APACP-982)

### 240206D-CMAP
- [x] [APACP-230](https://innate.atlassian.net/browse/APACP-230)
- [x] [APACP-976](https://innate.atlassian.net/browse/APACP-976)
- [x] [APACP-1119](https://innate.atlassian.net/browse/APACP-1119)

### 240305D-CMAP
- [ ] [APACP-948](https://innate.atlassian.net/browse/APACP-948)

### 240319D-CMAP
- [x] [APACP-1051](https://innate.atlassian.net/browse/APACP-1051)
- [x] [APACP-1066](https://innate.atlassian.net/browse/APACP-1066)
- [x] [APACP-1067](https://innate.atlassian.net/browse/APACP-1067)
- [x] [APACP-1068](https://innate.atlassian.net/browse/APACP-1068)
- [x] [APACP-1069](https://innate.atlassian.net/browse/APACP-1069)
- [x] [APACP-1070](https://innate.atlassian.net/browse/APACP-1070)
- [x] [APACP-1172](https://innate.atlassian.net/browse/APACP-1172)


| Element                    | Hide      | Primary Traveller Only | ... | End         | Mobile End  |
| -------------------------- | --------- | -------------------------------- | --- | ----------- | ----------- |
| Title                      | unchecked | checked                          |     | unchecked   | checked     |
| First name                 |           |                                  |     | checked     | checked     |
| Last name                  |           |                                  |     | unchecked   | checked     |
| Date of birth              |           |                                  |     | checked     | checked     |
| Email                      |           |                                  |     | unchecked   | checked     |
| Phone                      |           |                                  |     | checked     | checked     |
| <br>...<br>                |           |                                  |     |             |             |
| <br>Member Number & Suffix |           |                                  |     | <br>checked | <br>checked |
|                            |           |                                  |     |             |             |

Autocomplete address
Autocomplete address overrides
unchecked End

---
### 240402D-CMAP
- [ ] [APACP-1334](https://innate.atlassian.net/browse/APACP-1334) Quote Page: USP place holder - Desktop / Mobile  
- [ ] [APACP-1335](https://innate.atlassian.net/browse/APACP-1335) Quote Page: Customer service section- Desktop / Mobile
- [ ] [APACP-1337](https://innate.atlassian.net/browse/APACP-1337) Quote Page: Page footer / header - Desktop / Mobile 
- [ ] [APACP-1383](https://innate.atlassian.net/browse/APACP-1383) INC0308406: ROOT CAUSE REPAIR - Date Validation Error through API
- [ ] [APACP-1412](https://innate.atlassian.net/browse/APACP-1412) INC0317278: ahm - iFrame - Inaccessible symbol when selecting a date.


---
### 240416D-CMAP

|                                                              |                                                                    |
| ------------------------------------------------------------ | ------------------------------------------------------------------ |
| [APACP-1332](https://innate.atlassian.net/browse/APACP-1332) | Quote Page: Add Mozo awards on background image - Desktop / Mobile |
|                                                              |                                                                    |
| [APACP-1404](https://innate.atlassian.net/browse/APACP-1404) | [D] Add Apple Pay / Google Pay to BUPA                             |
