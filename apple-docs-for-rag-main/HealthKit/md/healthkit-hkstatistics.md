

- HealthKit
-  HKStatistics 

Class

# HKStatistics

An object that represents the result of calculating the minimum, maximum, average, or sum over a set of samples from the HealthKit store.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKStatistics
```

## Overview

HealthKit creates statistic objects using either a statistics query or a statistics collection query. For the statistics query, it performs the specified calculations over all the samples that match the query. For the statistics collection query, it partitions the matching samples into a set of time intervals and performs the calculations over each interval separately.

By default, these queries automatically merge the data from all of your data sources before performing the calculations. If you want to merge the data yourself, you can set the separateBySource option. You can then request the statistical data for each source separately.

When requesting data from a statistics object, your request must match the options you used when creating the query. For example, if you create a query using the discreteAverage option, you must access the results using the averageQuantity() method.

For more information on calculating statistical data, see HKStatisticsQuery Class Reference. To calculate the statistics over a series of time intervals, see the HKStatisticsCollectionQuery Class Reference.

## Topics

### Getting Property Data

var startDate: Date

The start of the time period included in these statistics.

var endDate: Date

The end of the time period included in these statistics.

var quantityType: HKQuantityType

The quantity type of the samples used to calculate these statistics.

var sources: [HKSource]?

An array containing all the sources contributing to these statistics.

### Getting Statistics Data

func averageQuantity() -> HKQuantity?

Returns the average value from all the samples that match the query.

func averageQuantity(for: HKSource) -> HKQuantity?

Returns the average value from all the samples that match the query and that were created by the specified source.

func maximumQuantity() -> HKQuantity?

Returns the maximum value from all the samples that match the query.

func maximumQuantity(for: HKSource) -> HKQuantity?

Returns the maximum value from all the samples that match the query and that were created by the specified source.

func minimumQuantity() -> HKQuantity?

Returns the minimum value from all the samples that match the query.

func minimumQuantity(for: HKSource) -> HKQuantity?

Returns the minimum value from all the samples that match the query and that were created by the specified source.

func sumQuantity() -> HKQuantity?

Returns the sum of all the samples that match the query.

func sumQuantity(for: HKSource) -> HKQuantity?

Returns the sum of all the samples that match the query and that were created by the specified source.

func duration() -> HKQuantity?

Returns the total duration covering all the samples that match the query.

func duration(for: HKSource) -> HKQuantity?

Returns the total duration covering all the samples created by the specified source that also match the query.

### Getting the Most Recent Quantity

func mostRecentQuantity() -> HKQuantity?

Returns the most recent value from all the samples that match the query.

func mostRecentQuantity(for: HKSource) -> HKQuantity?

Returns the most recent value from all the samples that match the query and were created by the specified source.

func mostRecentQuantityDateInterval() -> DateInterval?

Returns the date interval of the most recent sample that matches the query.

func mostRecentQuantityDateInterval(for: HKSource) -> DateInterval?

Returns the date interval of the most recent sample that matches the query and was created by the specified source.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
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

class HKStatisticsCollectionQuery

A query that performs multiple statistics queries over a series of fixed-length time intervals.

class HKStatisticsCollection

An object that manages a collection of statistics, representing the results calculated over separate time intervals.

struct HKStatisticsOptions

Options for specifying the statistic to calculate.

