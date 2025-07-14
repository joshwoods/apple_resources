

- HealthKit
- HKAnchoredObjectQueryDescriptor
-  result(for:) 

Instance Method

# result(for:)

Runs a one-shot query and asynchronously returns a snapshot of the current matching results.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
func result(for healthStore: HKHealthStore) async throws -> HKAnchoredObjectQueryDescriptor.Result
```

Available when `Sample` inherits `HKSample`.

## Parameters 

`healthStore`  

The access point for HealthKit data.

## See Also

### Running Queries

func results(for: HKHealthStore) -> HKAnchoredObjectQueryDescriptor&lt;Sample>.Results

Initiates a long-running query that returns its results using an asynchronous sequence.

struct Result

A set of results from an anchored object query.

struct Results

An asynchronous sequence that emits updates from an anchored object query.

