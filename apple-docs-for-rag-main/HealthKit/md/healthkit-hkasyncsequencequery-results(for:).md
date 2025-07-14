

- HealthKit
- HKAsyncSequenceQuery
-  results(for:) 

Instance Method

# results(for:)

Initiates a query that returns its results using an asynchronous sequence.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
func results(for healthStore: HKHealthStore) -> Self.Sequence
```

**Required**

## Parameters 

`healthStore`  

The access point for HealthKit data.

## Mentioned in 

Running Queries with Swift Concurrency

## Discussion

The adopting type’s Sequence associated type specifies the type of AsyncSequence that this method returns. For example, the HKAnchoredObjectQueryDescriptor returns an `HKAnchoredObjectQueryDescriptor/Sequence`, where each element in this sequence is an HKAnchoredObjectQueryDescriptor.Result value.

```
let anchorDescriptor =
HKAnchoredObjectQueryDescriptor(
    predicates: [.workout()],
    anchor: anchor)

let updateQueue = anchorDescriptor.results(for: store)

updateTask = Task {
    for try await results in updateQueue {
        // Process results here.
    }
}
```

Query descriptors for series data, like HKQuantitySeriesSampleQueryDescriptor, use an asynchronous sequence to return the high-frequency samples from a condensed sample, for example accessing individual heart rate samples from data recorded during a workout. These sequences have a finite size. When your app iterates over the sequence’s contents, the iteration automatically terminates after you receive all the data.

Other query descriptors, like HKAnchoredObjectQueryDescriptor, use this method to set up long-running queries that monitor the HealthKit store in the background. These queries continue to send updates using the asynchronous sequence. In these cases, code that iterates over the sequence continues until you cancel the sequence.

## See Also

### Running Queries

associatedtype Sequence : AsyncSequence

The data type that the query returns.

**Required**

