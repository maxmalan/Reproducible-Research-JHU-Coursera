Reproducible Research: Week 2 Assignment
========================================


## Loading and preprocessing the data.


```{r}
echo = TRUE
library(ggplot2)
library(dplyr)
activity <- read.csv("activity.csv", colClasses = c("integer", "Date", "factor"))
summary(activity)
str(activity)
head(activity)
tail(activity)
activity$month <- as.numeric(format(activity$date, "%m"))
```
