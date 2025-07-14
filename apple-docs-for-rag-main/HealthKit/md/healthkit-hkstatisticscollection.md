

- HealthKit
-  HKStatisticsCollection 

Class

# HKStatisticsCollection

An object that manages a collection of statistics, representing the results calculated over separate time intervals.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKStatisticsCollection
```

## Overview

For more information on statistics objects, see HKStatistics. For more information on calculating statistics over consecutive time intervals, see HKStatisticsCollectionQuery.

## Topics

### Accessing Statistics Collections

func statistics() -> [HKStatistics]

Returns an array of statistics objects representing the populated time intervals covered by the statistics collection query.

func statistics(for: Date) -> HKStatistics?

Returns the statistics object for the time interval that contains the provided date.

func enumerateStatistics(from: Date, to: Date, with: (HKStatistics, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates the statistics objects for all the time intervals from the start date until the end date.

### Getting Information About Statistics Collections

func sources() -> Set&lt;HKSource>

Returns a set containing all the sources that had samples matched by the statistics collection query.

## Relationships

### Inherits From

- NSObject

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

class HKStatisticsCollectionQuery

A query that performs multiple statistics queries over a series of fixed-length time intervals.

class HKStatistics

An object that represents the result of calculating the minimum, maximum, average, or sum over a set of samples from the HealthKit store.

struct HKStatisticsOptions

Options for specifying the statistic to calculate.

