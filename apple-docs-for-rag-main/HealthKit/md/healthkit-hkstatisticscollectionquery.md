

- HealthKit
-  HKStatisticsCollectionQuery 

Class

# HKStatisticsCollectionQuery

A query that performs multiple statistics queries over a series of fixed-length time intervals.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class HKStatisticsCollectionQuery
```

## Mentioned in 

Accessing condensed workout samples

Executing Statistics Collection Queries

## Overview

Statistics collection queries are often used to produce data for graphs and charts. For example, you might create a statistics collection query that calculates the total number of steps for each day or the average heart rate for each hour. Like observer queries, collection queries can also act as long-running queries, receiving updates when the HealthKit store’s content changes.

Important

You can only use statistics collection queries with quantity samples. If you want to calculate statistics over workouts or correlation samples, you must perform the appropriate query and process the data yourself.

Statistics collection queries are mostly immutable. You can assign the query’s initialResultsHandler and statisticsUpdateHandler properties after instantiating the object. You must set all other properties when you instantiate the object, and they can’t change.

For more information about statistics queries, see HKStatisticsQuery.

## Topics

### Creating Statistics Collection Objects

Executing Statistics Collection Queries

Calculate statistical data for graphs and charts.

init(quantityType: HKQuantityType, quantitySamplePredicate: NSPredicate?, options: HKStatisticsOptions, anchorDate: Date, intervalComponents: DateComponents)

Initializes a statistics collection query to perform the specified calculations over a set of time intervals.

### Getting and Setting Results Handlers

var initialResultsHandler: ((HKStatisticsCollectionQuery, HKStatisticsCollection?, (any Error)?) -> Void)?

The results handler for the query’s initial results.

var statisticsUpdateHandler: ((HKStatisticsCollectionQuery, HKStatistics?, HKStatisticsCollection?, (any Error)?) -> Void)?

The results handler for monitoring updates to the HealthKit store.

### Getting Property Data

var anchorDate: Date

The anchor date for the collection’s time intervals.

var intervalComponents: DateComponents

The date components that define the time interval for each statistics object in the collection.

var options: HKStatisticsOptions

A list of options that define the type of statistical calculations performed and the way in which data from multiple sources are merged.

## Relationships

### Inherits From

- HKQuery

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Statistics

Executing Statistical Queries

Create and run statistical queries.

Executing Statistics Collection Queries

Calculate statistical data for graphs and charts.

struct HKStatisticsQueryDescriptor

A query descriptor that calculates the minimum, maximum, average, or sum over a set of samples from the HealthKit store.

class HKStatisticsQuery

A query that performs statistical calculations over a set of matching quantity samples, and returns the results.

struct HKStatisticsCollectionQueryDescriptor

A query descriptor that gathers a collection of statistics calculated over a series of fixed-length time intervals.

class HKStatistics

An object that represents the result of calculating the minimum, maximum, average, or sum over a set of samples from the HealthKit store.

class HKStatisticsCollection

An object that manages a collection of statistics, representing the results calculated over separate time intervals.

struct HKStatisticsOptions

Options for specifying the statistic to calculate.

