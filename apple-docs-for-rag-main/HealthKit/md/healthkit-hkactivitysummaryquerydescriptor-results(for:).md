

- HealthKit
- HKActivitySummaryQueryDescriptor
-  results(for:) 

Instance Method

# results(for:)

Initiates a long-running query that returns its results using an asynchronous sequence.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
func results(for healthStore: HKHealthStore) -> HKActivitySummaryQueryDescriptor.Results
```

## Parameters 

`healthStore`  

The access point for HealthKit data.

## See Also

### Running queries

func result(for: HKHealthStore) async throws -> [HKActivitySummary]

Runs a one-shot query and asynchronously returns a snapshot of the current matching results.

struct Results

An asynchronous sequence that emits updates from an activity summary query.

