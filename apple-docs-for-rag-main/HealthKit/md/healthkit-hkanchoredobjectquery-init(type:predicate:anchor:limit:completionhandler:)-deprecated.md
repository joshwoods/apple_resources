

- HealthKit
- HKAnchoredObjectQuery
-  init(type:predicate:anchor:limit:completionHandler:) Deprecated

Initializer

# init(type:predicate:anchor:limit:completionHandler:)

Initializes a new anchored object query.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOSvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
init(
    type: HKSampleType,
    predicate: NSPredicate?,
    anchor: Int,
    limit: Int,
    completionHandler handler: @escaping (HKAnchoredObjectQuery, [HKSample]?, Int, (any Error)?) -> Void
)
```

Deprecated

This method is deprecated. Use init(type:predicate:anchor:limit:resultsHandler:) instead.

## Parameters 

`type`  

The type of sample to search for. This query supports all sample types. Specifically, you can pass any concrete subclass of the HKSampleType class (the HKQuantityType, HKCategoryType, HKWorkoutType, and HKCorrelationType classes).

`predicate`  

A predicate that filters the samples returned by the query. Pass `nil` to receive all the new samples of the specified type.

`anchor`  

The anchor returned by the previous anchored object query. The anchor value corresponds to the last sample that was returned by the previous anchored object query. The new query returns only objects newer than that sample.

`limit`  

The maximum number of samples received by the query. To receive all of the new samples, pass HKObjectQueryNoLimit.

`handler`  

A block that is called when the query finishes executing. This block takes the following parameters:

query  
A reference to the query calling this block.

results  
An array containing the samples returned by this query, or `nil` if an error occurred.

newAnchor  
A value corresponding to the last sample in the results array. Subsequent anchor queries can use this value to receive only the samples that have been saved and the objects that have been deleted since this query completed.

error  
If an error occurs, this parameter contains an object describing the error; otherwise, it is `nil`.

## Return Value

A newly initialized anchor query object.

## Discussion

After instantiating the query, call the HKHealthStore class’s execute(_:) method to run it. The queries run on an anonymous background queue. As soon as the query is complete, the handler is executed on the same background queue (but not necessarily the same thread).

## Topics

### Constants

var HKAnchoredObjectQueryNoAnchor: Int32

An anchor that returns all of the matching samples currently in the HealthKit store.

## See Also

### Creating Anchored Object Queries

Executing Anchored Object Queries

Create and run an anchored object query.

init(type: HKSampleType, predicate: NSPredicate?, anchor: HKQueryAnchor?, limit: Int, resultsHandler: (HKAnchoredObjectQuery, [HKSample]?, [HKDeletedObject]?, HKQueryAnchor?, (any Error)?) -> Void)

Initializes a new anchored object query.

init(queryDescriptors: [HKQueryDescriptor], anchor: HKQueryAnchor?, limit: Int, resultsHandler: (HKAnchoredObjectQuery, [HKSample]?, [HKDeletedObject]?, HKQueryAnchor?, (any Error)?) -> Void)

Creates an anchored object query that matches any of the query descriptors you provided.

let HKObjectQueryNoLimit: Int

A value indicating that the query returns all the matching samples in the HealthKit store.

