

- HealthKit
- HKStatisticsCollectionQueryDescriptor
-  HKStatisticsCollectionQueryDescriptor.Results 

Structure

# HKStatisticsCollectionQueryDescriptor.Results

An asynchronous sequence that emits updates from a statistics collection query.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct Results
```

## Topics

### Creating an Iterator

struct Iterator

An iterator for statistics collection query results.

struct Result

A collection of results.

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Running Queries

func result(for: HKHealthStore) async throws -> HKStatisticsCollection

Runs a one-shot query and asynchronously returns statistics calculated from the current matching results.

func results(for: HKHealthStore) -> HKStatisticsCollectionQueryDescriptor.Results

Initiates a long-running query that returns statistics and updates using an asynchronous sequence.

