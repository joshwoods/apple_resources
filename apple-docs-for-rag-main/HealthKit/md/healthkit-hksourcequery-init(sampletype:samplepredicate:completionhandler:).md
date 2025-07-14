

- HealthKit
- HKSourceQuery
-  init(sampleType:samplePredicate:completionHandler:) 

Initializer

# init(sampleType:samplePredicate:completionHandler:)

Instantiates and returns a source query.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
init(
    sampleType: HKSampleType,
    samplePredicate objectPredicate: NSPredicate?,
    completionHandler: @escaping (HKSourceQuery, Set?, (any Error)?) -> Void
)
```

## Parameters 

`sampleType`  

The type of sample to search for. This query supports all sample types. Specifically, you can pass any concrete subclass of the HKSampleType class (the HKQuantityType, HKCategoryType, HKWorkoutType, and HKCorrelationType classes).

`objectPredicate`  

A predicate that limits the samples matched by the query. Pass `nil` if you want to receive the sources for all the samples of the specified type.

`completionHandler`  

A block that is called when the query finishes executing. This block takes the following parameters:

query  
A reference to the query calling this block.

results  
A set containing the sources for all the samples that match both the sample type and the object predicate, or `nil` if an error occurred.

error  
If an error occurs, this parameter contains an object describing the error; otherwise, it is `nil`.

## Return Value

A newly initialized sample query object.

## Mentioned in 

Executing Source Queries

## Discussion

After instantiating the query, call the HKHealthStore class’s execute(_:) method to run this query. Queries run on an anonymous background queue. As soon as the query is complete, the results handler is executed on the same background queue (but not necessarily on the same thread).

## See Also

### Creating Source Queries

Executing Source Queries

Create and run source queries.

