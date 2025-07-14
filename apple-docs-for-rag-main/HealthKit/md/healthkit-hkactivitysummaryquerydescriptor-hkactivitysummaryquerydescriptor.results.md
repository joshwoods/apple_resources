

- HealthKit
- HKActivitySummaryQueryDescriptor
-  HKActivitySummaryQueryDescriptor.Results 

Structure

# HKActivitySummaryQueryDescriptor.Results

An asynchronous sequence that emits updates from an activity summary query.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct Results
```

## Topics

### Creating an Iterator

struct Iterator

An iterator for accessing active summary results.

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Running queries

func result(for: HKHealthStore) async throws -> [HKActivitySummary]

Runs a one-shot query and asynchronously returns a snapshot of the current matching results.

func results(for: HKHealthStore) -> HKActivitySummaryQueryDescriptor.Results

Initiates a long-running query that returns its results using an asynchronous sequence.

