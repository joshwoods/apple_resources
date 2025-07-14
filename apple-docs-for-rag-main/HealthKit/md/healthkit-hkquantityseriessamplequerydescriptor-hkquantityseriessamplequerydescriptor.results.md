

- HealthKit
- HKQuantitySeriesSampleQueryDescriptor
-  HKQuantitySeriesSampleQueryDescriptor.Results 

Structure

# HKQuantitySeriesSampleQueryDescriptor.Results

An asynchronous sequence that emits data from the quantity series query.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct Results
```

## Topics

### Creating an Iterator

struct Iterator

An iterator for accessing individual data entries from the series.

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Running Queries

func results(for: HKHealthStore) -> HKQuantitySeriesSampleQueryDescriptor.Results

Runs a one-shot query that returns an asynchronous sequence of matching series samples.

struct Result

A set of results from a quantity series sample descriptor.

