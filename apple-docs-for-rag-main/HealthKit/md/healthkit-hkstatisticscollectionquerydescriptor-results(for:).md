

- HealthKit
- HKStatisticsCollectionQueryDescriptor
-  results(for:) 

Instance Method

# results(for:)

Initiates a long-running query that returns statistics and updates using an asynchronous sequence.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
func results(for healthStore: HKHealthStore) -> HKStatisticsCollectionQueryDescriptor.Results
```

## Parameters 

`healthStore`  

The access point for HealthKit data.

## See Also

### Running Queries

func result(for: HKHealthStore) async throws -> HKStatisticsCollection

Runs a one-shot query and asynchronously returns statistics calculated from the current matching results.

struct Results

An asynchronous sequence that emits updates from a statistics collection query.

