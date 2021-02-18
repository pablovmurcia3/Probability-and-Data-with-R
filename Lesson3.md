---
title: "Lesson3"
output: 
  html_document: 
    keep_md: yes
---



## **Exploring Categorical variables**

### **Frequency table and bar plot**


```r
table(mtcars$cyl)
```

```
## 
##  4  6  8 
## 11  7 14
```

```r
barplot(table(mtcars$cyl))
```

<img src="Lesson3_files/figure-html/n-1.png" style="display: block; margin: auto;" />

*barplot* different form *histogram*

### **Contingency table**


```r
data(UCBAdmissions)
DF <- as.data.frame(UCBAdmissions)
xt <- xtabs(Freq ~ Gender + Admit,data=DF) # CROSS TAB
xt
```

```
##         Admit
## Gender   Admitted Rejected
##   Male       1198     1493
##   Female      557     1278
```

### **segmented barplot**


```r
barplot(xt)
```

<img src="Lesson3_files/figure-html/dd4-1.png" style="display: block; margin: auto;" />

Visualizing conditional frequency distribution 

the alternative is calculate relative frequency segment barplot

### **Mosaicplot**

### **side-by-side boxplot**


```r
data("airquality")
library(dplyr)
```

```
## 
## Attaching package: 'dplyr'
```

```
## The following objects are masked from 'package:stats':
## 
##     filter, lag
```

```
## The following objects are masked from 'package:base':
## 
##     intersect, setdiff, setequal, union
```

```r
airquality <- mutate(airquality, Month = factor(Month)) 
boxplot(Ozone ~ Month, airquality, xlab = "Month", ylab = "Ozone (ppb)")
```

<img src="Lesson3_files/figure-html/da-1.png" style="display: block; margin: auto;" />


