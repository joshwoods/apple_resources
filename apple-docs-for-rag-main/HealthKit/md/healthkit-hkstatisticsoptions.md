

- HealthKit
-  HKStatisticsOptions 

Structure

# HKStatisticsOptions

Options for specifying the statistic to calculate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
struct HKStatisticsOptions
```

## Overview

You cannot combine a discrete option with a cumulative option. You can, however, combine multiple discrete options together to perform multiple calculations. You can also combine the separateBySource option with any of the other options.

## Swift

```
let cumulativeActiveEnergyBurned =
    HKObjectType.quantityTypeForIdentifier(HKQuantityTypeIdentifierActiveEnergyBurned)

let discreteHeartRate =
    HKObjectType.quantityTypeForIdentifier(HKQuantityTypeIdentifierHeartRate)

// Cannot combine cumulative options with discrete options.
// However, you can combine a cumulative option and seperated by source
let cumulativeQuery = HKStatisticsQuery(quantityType:cumulativeActiveEnergyBurned,
                                        quantitySamplePredicate:nil,
                                        options: .CumulativeSum | .SeparateBySource) {
                                            query, statistics, error in

                                            // ... process the results here
}

// You can also combine any number of discrete options
// and the seperated by source option.
let discreteQuery = HKStatisticsQuery(quantityType: discreteHeartRate,
                                      quantitySamplePredicate: nil,
                                      options: .DiscreteAverage | .DiscreteMin |
                                        .DiscreteMax | .SeparateBySource) {
                                            query, statistics, error in

                                            // ... process the results here
}
```

## Objective-C

```
HKQuantityType *cumulativeActiveEnergyBurned =
[HKObjectType quantityTypeForIdentifier:HKQuantityTypeIdentifierActiveEnergyBurned];

HKQuantityType *discreteHeartRate =
[HKObjectType quantityTypeForIdentifier:HKQuantityTypeIdentifierHeartRate];

// Cannot combine cumulative options with discrete options.
// However, you can combine a cumulative option and seperated by source
HKStatisticsQuery *cumulativeQuery =
[[HKStatisticsQuery alloc]
 initWithQuantityType:cumulativeActiveEnergyBurned
 quantitySamplePredicate:nil
 options:HKStatisticsOptionCumulativeSum | HKStatisticsOptionSeparateBySource
 completionHandler:^(HKStatisticsQuery *query, HKStatistics *result, NSError *error) {

      // ... process the results here
 }];

// You can also combine any number of discrete options
// and the seperated by source option.
HKStatisticsQuery *discreteQuery =
[[HKStatisticsQuery alloc]
 initWithQuantityType:discreteHeartRate
 quantitySamplePredicate:nil
 options:HKStatisticsOptionDiscreteAverage | HKStatisticsOptionDiscreteMin |
 HKStatisticsOptionDiscreteMax | HKStatisticsOptionSeparateBySource
 completionHandler:^(HKStatisticsQuery *query, HKStatistics *result, NSError *error) {

     // ... process the results here
 }];
```

## Topics

### Constants

static var separateBySource: HKStatisticsOptions

An option indicating that the system calculates the specified statistics separately for each source.

static var discreteAverage: HKStatisticsOptions

An option indicating that the system calculates the average quantity for the samples.

static var discreteMin: HKStatisticsOptions

An option indicating that the system calculates the minimum quantity for the samples.

static var discreteMax: HKStatisticsOptions

An option indicating that the system calculates the maximum quantity for the samples.

static var cumulativeSum: HKStatisticsOptions

An option indicating that the system calculates the sum of all the quantities for the samples.

static var mostRecent: HKStatisticsOptions

An option indicating that the system returns the most recent quantity from the matching samples.

static var duration: HKStatisticsOptions

An option indicating that the system calculates the total duration covering all the samples.

### Deprecated Constants

static var discreteMostRecent: HKStatisticsOptions

An option indicating that the system returns the most recent quantity from the matching samples.

Deprecated

### Initializers

init(rawValue: UInt)

Returns a newly initialized statistics option using the provided integer.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

class HKStatisticsCollection

An object that manages a collection of statistics, representing the results calculated over separate time intervals.

