

- HealthKit
- HKAsyncSequenceQuery
-  Sequence 

Associated Type

# Sequence

The data type that the query returns.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
associatedtype Sequence : AsyncSequence
```

**Required**

## See Also

### Running Queries

func results(for: HKHealthStore) -> Self.Sequence

Initiates a query that returns its results using an asynchronous sequence.

**Required**

