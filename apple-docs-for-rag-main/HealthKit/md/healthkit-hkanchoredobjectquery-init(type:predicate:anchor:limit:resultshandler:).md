

- HealthKit
- HKAnchoredObjectQuery
-  init(type:predicate:anchor:limit:resultsHandler:) 

Initializer

# init(type:predicate:anchor:limit:resultsHandler:)

Initializes a new anchored object query.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    type: HKSampleType,
    predicate: NSPredicate?,
    anchor: HKQueryAnchor?,
    limit: Int,
    resultsHandler handler: @escaping (HKAnchoredObjectQuery, [HKSample]?, [HKDeletedObject]?, HKQueryAnchor?, (any Error)?) -> Void
)
```

## Parameters 

`type`  

The type of sample to search for. This query supports all subclasses of HKSampleType, such as HKQuantityType, HKCategoryType, HKWorkoutType, and HKCorrelationType.

`predicate`  

A predicate that filters both the samples and the deleted objects returned by the query. Pass `nil` to receive all the newly added samples and recently deleted objects of the specified type.

`anchor`  

The anchor returned by the previous anchored object query. The anchor object corresponds to the last object that was returned by the previous anchored object query. The new query returns only samples and deleted objects that are newer than that object.

Pass `nil` to receive all the matching samples and recently deleted objects currently in the HealthKit store.

`limit`  

The maximum number of samples received by the query. To receive all of the new samples, pass HKObjectQueryNoLimit.

`handler`  

A block that the system calls after gathering the initial results. This block takes the following parameters:

query  
A reference to the query calling this block.

sampleObjects  
An array containing the samples returned by this query, or `nil` if an error occurred.

deletedObjects  
An array containing the deleted objects returned by this query, or `nil` if an error occurred.

newAnchor  
An anchor object corresponding to the last object returned by this query. Subsequent anchor queries use this value to receive new samples and deleted objects created after the query returned its initial results.

error  
If an error occurs, this parameter contains an object describing the error; otherwise, it is `nil`.

## Return Value

A newly initialized anchor query object.

## Mentioned in 

Executing Anchored Object Queries

## Discussion

After instantiating the query, call the HKHealthStore class’s execute(_:) method to run it. The queries run on an anonymous background queue. As soon as the query is complete, the results handler block is executed on the same background queue (but not necessarily the same thread). Be sure to dispatch these results to the main queue before updating the user interface.

The first time you call this method, pass `nil` as the `anchor` parameter. This method returns all matching objects currently in the HealthKit store. Additionally, save the returned anchor object and pass it to the next query.

Anchor queries can also act as long-running queries. If you assign an update handler before executing the query, the query continues to monitor the HealthKit store after gathering the initial results. The system calls the update handler on a background queue whenever a matching sample is saved to or deleted from the HealthKit store. To cancel this query, call the store’s stop(_:) method.

## See Also

### Creating Anchored Object Queries

Executing Anchored Object Queries

Create and run an anchored object query.

init(queryDescriptors: [HKQueryDescriptor], anchor: HKQueryAnchor?, limit: Int, resultsHandler: (HKAnchoredObjectQuery, [HKSample]?, [HKDeletedObject]?, HKQueryAnchor?, (any Error)?) -> Void)

Creates an anchored object query that matches any of the query descriptors you provided.

let HKObjectQueryNoLimit: Int

A value indicating that the query returns all the matching samples in the HealthKit store.

init(type: HKSampleType, predicate: NSPredicate?, anchor: Int, limit: Int, completionHandler: (HKAnchoredObjectQuery, [HKSample]?, Int, (any Error)?) -> Void)

Initializes a new anchored object query.

Deprecated

