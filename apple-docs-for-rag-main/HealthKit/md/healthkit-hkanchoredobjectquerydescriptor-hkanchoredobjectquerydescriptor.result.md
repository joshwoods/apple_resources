

- HealthKit
- HKAnchoredObjectQueryDescriptor
-  HKAnchoredObjectQueryDescriptor.Result 

Structure

# HKAnchoredObjectQueryDescriptor.Result

A set of results from an anchored object query.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct Result
```

## Topics

### Accessing the Results

let addedSamples: [Sample]

An array containing the matching samples added to the HealthKit store.

let deletedObjects: [HKDeletedObject]

An array of objects deleted from the HealthKit store.

let newAnchor: HKQueryAnchor

A value corresponding to the last sample that the anchor query has returned.

## See Also

### Running Queries

func result(for: HKHealthStore) async throws -> HKAnchoredObjectQueryDescriptor&lt;Sample>.Result

Runs a one-shot query and asynchronously returns a snapshot of the current matching results.

func results(for: HKHealthStore) -> HKAnchoredObjectQueryDescriptor&lt;Sample>.Results

Initiates a long-running query that returns its results using an asynchronous sequence.

struct Results

An asynchronous sequence that emits updates from an anchored object query.

