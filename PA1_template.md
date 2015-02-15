Reproducible Research: Peer Assignment 1
========================================================

## Loading and preprocessing the data



```r
activity <- read.csv("activity.csv")
```

```
## Warning: cannot open file 'activity.csv': No such file or directory
```

```
## Error: cannot open the connection
```

```r
activity <- transform(activity, date = as.Date(date, "%Y-%m-%d"))
```

```
## Error: object 'activity' not found
```

```r
total = aggregate(activity$steps ~ activity$date, activity, sum)
```

```
## Error: object 'activity' not found
```


## What is mean total number of steps taken per day?


### Histogram

The histogram of the number of steps taken per day is shown below.

```r
library(lattice)
# Draw a histogram of the total number of steps taken each day
histogram(total[,2], xlab = "Number of steps", main="Histogram of Number of steps taken each day")
```

```
## Error: object 'total' not found
```















