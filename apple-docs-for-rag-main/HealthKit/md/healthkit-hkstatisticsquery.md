

- HealthKit
-  HKStatisticsQuery 

Class

# HKStatisticsQuery

A query that performs statistical calculations over a set of matching quantity samples, and returns the results.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class HKStatisticsQuery
```

## Mentioned in 

Accessing condensed workout samples

Executing Statistics Collection Queries

## Overview

Statistics queries calculate common statistics over the set of matching samples. You can use statistical queries to calculate the minimum, maximum, or average value of a set of discrete quantities, or use them to calculate the sum for cumulative quantities. For the complete list of possible calculations, see HKStatisticsOptions. For more information about the available quantity types and to learn whether they are discrete or cumulative values, see Data types.

You can use statistics queries with quantity samples only. If you want to calculate statistics over workouts or correlation samples, you must perform the appropriate query and process the data yourself.

Statistics queries are immutable. Their properties are set when they are first created, and they can’t change.

## Topics

### Creating Statistics Queries

init(quantityType: HKQuantityType, quantitySamplePredicate: NSPredicate?, options: HKStatisticsOptions, completionHandler: (HKStatisticsQuery, HKStatistics?, (any Error)?) -> Void)

Initializes a statistics query instance that performs the specified calculations over the matching samples in the HeathKit store.

Executing Statistical Queries

Create and run statistical queries.

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

struct HKStatisticsCollectionQueryDescriptor

A query descriptor that gathers a collection of statistics calculated over a series of fixed-length time intervals.

class HKStatisticsCollectionQuery

A query that performs multiple statistics queries over a series of fixed-length time intervals.

class HKStatistics

An object that represents the result of calculating the minimum, maximum, average, or sum over a set of samples from the HealthKit store.

class HKStatisticsCollection

An object that manages a collection of statistics, representing the results calculated over separate time intervals.

struct HKStatisticsOptions

Options for specifying the statistic to calculate.

