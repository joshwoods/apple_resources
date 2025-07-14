

- HealthKit
- HKQuantitySeriesSampleQueryDescriptor
-  results(for:) 

Instance Method

# results(for:)

Runs a one-shot query that returns an asynchronous sequence of matching series samples.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
func results(for healthStore: HKHealthStore) -> HKQuantitySeriesSampleQueryDescriptor.Results
```

## Parameters 

`healthStore`  

The access point for HealthKit data.

## See Also

### Running Queries

struct Results

An asynchronous sequence that emits data from the quantity series query.

struct Result

A set of results from a quantity series sample descriptor.

