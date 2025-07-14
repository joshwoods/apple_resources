

- HealthKit
- HKStatisticsCollectionQueryDescriptor
-  HKStatisticsCollectionQueryDescriptor.Result 

Structure

# HKStatisticsCollectionQueryDescriptor.Result

A collection of results.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct Result
```

## Overview

The first set of results reflects the current state of the statistics collection. Additional results represent updates to the collection. When possible, HealthKit populates the `updateStatistics` property to indicate which statistics have changed.

## Topics

### Accessing Statistical Data

let statisticsCollection: HKStatisticsCollection

A collection of statistics, representing the results calculated over separate time intervals.

let updatedStatistics: [HKStatistics]?

A collection of statistics that have changed.

## See Also

### Creating an Iterator

struct Iterator

An iterator for statistics collection query results.

