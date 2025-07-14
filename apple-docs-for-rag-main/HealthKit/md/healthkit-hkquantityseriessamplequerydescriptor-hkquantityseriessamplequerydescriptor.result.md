

- HealthKit
- HKQuantitySeriesSampleQueryDescriptor
-  HKQuantitySeriesSampleQueryDescriptor.Result 

Structure

# HKQuantitySeriesSampleQueryDescriptor.Result

A set of results from a quantity series sample descriptor.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct Result
```

## Topics

### Accessing Sample Data

let sample: HKQuantitySample?

The quantity sample that owns the series of data entries.

let quantity: HKQuantity

The quantity stored by the data entry.

let dateInterval: DateInterval

The date interval for the entry.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Running Queries

func results(for: HKHealthStore) -> HKQuantitySeriesSampleQueryDescriptor.Results

Runs a one-shot query that returns an asynchronous sequence of matching series samples.

struct Results

An asynchronous sequence that emits data from the quantity series query.

