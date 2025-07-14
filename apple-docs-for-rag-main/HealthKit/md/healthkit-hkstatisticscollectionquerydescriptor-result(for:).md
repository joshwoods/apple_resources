

- HealthKit
- HKStatisticsCollectionQueryDescriptor
-  result(for:) 

Instance Method

# result(for:)

Runs a one-shot query and asynchronously returns statistics calculated from the current matching results.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
func result(for healthStore: HKHealthStore) async throws -> HKStatisticsCollection
```

## Parameters 

`healthStore`  

The access point for HealthKit data.

## See Also

### Running Queries

func results(for: HKHealthStore) -> HKStatisticsCollectionQueryDescriptor.Results

Initiates a long-running query that returns statistics and updates using an asynchronous sequence.

struct Results

An asynchronous sequence that emits updates from a statistics collection query.

