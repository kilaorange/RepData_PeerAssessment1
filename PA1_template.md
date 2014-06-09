# Reproducible Research: Peer Assessment 1


## Loading and preprocessing the data
Set the working directory:

```r
setwd("~/Documents/Coursera/dataScienceSpecialisation/RepData_PeerAssessment1")
```


Read in the data:

```r
data <- read.csv("activity.csv")
```


Do some transformations to get the data ready for analysis:



## What is mean total number of steps taken per day?
Histogram of total number of steps taken each day:

```r
require(ggplot2)
```

```
## Loading required package: ggplot2
```

```r
plot <- ggplot(someData, aes(x = vaiable)) + geom_histogram(aes(y = ..something..))
```

```
## Error: object 'someData' not found
```


The mean and median total number of steps taken per day are:
| Summary   | Value        | 
| ----------|-------------:|
| Mean      | 'r myMean'   |
| Median    | 'r myMedian' |


## What is the average daily activity pattern?
### Time Series Plot
5min intervals and average number of steps taken in each 5min, averaged across all days.
Do something about the missing values (remove or approximate using impute)

5min interval that contains the max AVG number of steps??


## Imputing missing values
Calculate the total number of missing values in dataset.

```r
missingVals <- nrow(data[which(is.na(data$steps) == TRUE), ])
missingVals
```

```
## [1] 2304
```

Total number of missing = 2304

### Fill in the missing numbers and save as a new dataset

```r
require(impute)
```

```
## Loading required package: impute
```

```r

```


### Histogram of Total number of steps taken each day

```r
require(ggplot2)
plot <- ggplot(someData, aes(x = vaiable)) + geom_histogram(aes(y = ..something..))
```

```
## Error: object 'someData' not found
```



The mean and median total number of steps taken per day are:
| Summary   | Value        | 
| ----------|-------------:|
| Mean      | 'r myMean'   |
| Median    | 'r myMedian' |

### Effects of Imputing Missing Values on estimates of daily number of steps

## Are there differences in activity patterns between weekdays and weekends?
- Use weekdays() function
- Use dataset with filled in values

1. Create new factor in dataset with 2 levels "Weekday", "Weekend"
2. Make time series panel plot (type "l") x-axis = 5min interval, y-axis = avg steps taken
























