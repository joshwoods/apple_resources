

- HealthKit
- HKAnchoredObjectQueryDescriptor
-  HKAnchoredObjectQueryDescriptor.Results 

Structure

# HKAnchoredObjectQueryDescriptor.Results

An asynchronous sequence that emits updates from an anchored object query.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct Results
```

Available when `Sample` inherits `HKSample`.

## Topics

### Creating an Iterator

struct Iterator

An iterator for accessing anchored object results.

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Running Queries

func result(for: HKHealthStore) async throws -> HKAnchoredObjectQueryDescriptor&lt;Sample>.Result

Runs a one-shot query and asynchronously returns a snapshot of the current matching results.

func results(for: HKHealthStore) -> HKAnchoredObjectQueryDescriptor&lt;Sample>.Results

Initiates a long-running query that returns its results using an asynchronous sequence.

struct Result

A set of results from an anchored object query.

