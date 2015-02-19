---
title       : Shiny app to find cost of medical procedure in your area (in US)
subtitle    : 
author      : Piyush Madan
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Intro

This shiny app will help you to find cost of different incare medical procedures in your state. You can compare and select one that is fitting your needs

In this app, I'm filtering on Procedure name & State from a large dataset from Data.CMS.gov . User can filter results from filters on result table

Data Source: 
https://data.cms.gov/Medicare/Inpatient-Prospective-Payment-System-IPPS-Provider/97k6-zzx3

Github: 
https://github.com/piyushmadan/ShinyAppDemo

Shiny App: 
https://piyushmadan.shinyapps.io/ShinyDemoApp


---
## Information about Data
Source: [Data.CMS.gov](https://data.cms.gov/Medicare/Inpatient-Prospective-Payment-System-IPPS-Provider/97k6-zzx3)


```r
  data <- read.csv("Inpatient_Prospective_Payment_System__IPPS__Provider_Summary_for_the_Top_100_Diagnosis-Related_Groups__DRG__-_FY2011.csv")
  names(data)
```

```
##  [1] "DRG.Definition"                      
##  [2] "Provider.Id"                         
##  [3] "Provider.Name"                       
##  [4] "Provider.Street.Address"             
##  [5] "Provider.City"                       
##  [6] "Provider.State"                      
##  [7] "Provider.Zip.Code"                   
##  [8] "Hospital.Referral.Region.Description"
##  [9] "Total.Discharges"                    
## [10] "Average.Covered.Charges"             
## [11] "Average.Total.Payments"              
## [12] "Average.Medicare.Payments"
```

---

## Get Started with Demo (iframe)
Wait for app to be downloaded below this text. If iframe doesn't not load/ fit properly on your screen, visit [Shiny App](https://piyushmadan.shinyapps.io/ShinyDemoApp/ "ShinyApp"). Once app is loaded select (multiple) states and procedure. Wait for record to be updated. Use search/filter in options to figure out best place to go for that procedure
<iframe src="https://piyushmadan.shinyapps.io/ShinyDemoApp/" style=></iframe>


--- 
## Files in project

Link to Github: https://github.com/piyushmadan/ShinyAppDemo

- [ui.R](https://github.com/piyushmadan/ShinyAppDemo/blob/master/ui.R)
- [server.R](https://github.com/piyushmadan/ShinyAppDemo/blob/master/server.R)
- [ReadMe.md](https://github.com/piyushmadan/ShinyAppDemo/blob/master/ReadMe.md)
- [DataFile](https://github.com/piyushmadan/ShinyAppDemo/blob/master/Inpatient_Prospective_Payment_System__IPPS__Provider_Summary_for_the_Top_100_Diagnosis-Related_Groups__DRG__-_FY2011.csv)

## References

- http://shiny.rstudio.com/tutorial/
- http://shiny.rstudio.com/reference/shiny/latest/
- Inpatient Prospective Payment System (IPPS) Provider Summary for the Top 100 Diagnosis-Related Groups (DRG) from https://data.cms.gov/




