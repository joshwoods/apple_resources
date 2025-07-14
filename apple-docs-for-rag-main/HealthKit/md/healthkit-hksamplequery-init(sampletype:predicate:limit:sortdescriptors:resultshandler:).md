

- HealthKit
- HKSampleQuery
-  init(sampleType:predicate:limit:sortDescriptors:resultsHandler:) 

Initializer

# init(sampleType:predicate:limit:sortDescriptors:resultsHandler:)

Instantiates and returns a sample query.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
init(
    sampleType: HKSampleType,
    predicate: NSPredicate?,
    limit: Int,
    sortDescriptors: [NSSortDescriptor]?,
    resultsHandler: @escaping (HKSampleQuery, [HKSample]?, (any Error)?) -> Void
)
```

## Parameters 

`sampleType`  

The type of sample to search for. This object can be an instance of the HKCategoryType, HKCorrelationType, HKQuantityType, or HKWorkoutType class.

`predicate`  

A predicate that limits the results returned by the query. Pass `nil` to receive all the samples of the specified type.

`limit`  

The maximum number of samples returned by the query. If you want to return all matching samples, use HKObjectQueryNoLimit.

`sortDescriptors`  

An array of sort descriptors that specify the order of the results returned by this query. Pass `nil` if you don’t need the results in a specific order.

Note

HealthKit defines a number of sort identifiers (for example, HKSampleSortIdentifierStartDate and HKWorkoutSortIdentifierDuration). Use the sort descriptors you create with these identifiers only in queries. You cannot use them to perform an in-memory sort of an array of samples.

`resultsHandler`  

A block that is called when the query finishes executing.

This block takes the following parameters:

query  
A reference to the query that called this block.

results  
An array containing the samples found by the query, or `nil` if an error occurs.

error  
If an error occurs, this parameter contains an object describing the error. Otherwise, its value is `nil`.

## Return Value

A newly initialized sample query object.

## Mentioned in 

Executing Sample Queries

## Discussion

After instantiating the query, call the HKHealthStore class’s execute(_:) method to run this query. Queries run on an anonymous background queue. As soon as the query is complete, the results handler is executed on the background queue. You typically dispatch these results to the main queue to update the user interface.

## See Also

### Creating Sample Queries

Executing Sample Queries

Create, run, and sort sample queries.

init(queryDescriptors: [HKQueryDescriptor], limit: Int, resultsHandler: (HKSampleQuery, [HKSample]?, (any Error)?) -> Void)

Creates a query for samples that match any of the descriptors you provided.

init(queryDescriptors: [HKQueryDescriptor], limit: Int, sortDescriptors: [NSSortDescriptor], resultsHandler: (HKSampleQuery, [HKSample]?, (any Error)?) -> Void)

Creates a query for samples that match any of the query descriptors you provided, sorted by the sort descriptors you provided.

let HKObjectQueryNoLimit: Int

A value indicating that the query returns all the matching samples in the HealthKit store.

HealthKit sort descriptors

Identifiers for sorting results.

