

- HealthKit
- HKSampleQuery
-  init(queryDescriptors:limit:sortDescriptors:resultsHandler:) 

Initializer

# init(queryDescriptors:limit:sortDescriptors:resultsHandler:)

Creates a query for samples that match any of the query descriptors you provided, sorted by the sort descriptors you provided.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    queryDescriptors: [HKQueryDescriptor],
    limit: Int,
    sortDescriptors: [NSSortDescriptor],
    resultsHandler: @escaping (HKSampleQuery, [HKSample]?, (any Error)?) -> Void
)
```

## Parameters 

`queryDescriptors`  

An array of descriptors that specify the types of samples that the query returns.

`limit`  

The maximum number of samples that the query returns. If you want to return all matching samples, use HKObjectQueryNoLimit.

`sortDescriptors`  

An array of sort descriptors that specify the order of the results that the query returns.

Note

HealthKit defines a number of sort identifiers (for example, HKSampleSortIdentifierStartDate and HKWorkoutSortIdentifierDuration). Use the sort descriptors you create with these identifiers only in queries. You can’t use them to perform an in-memory sort of an array of samples.

`resultsHandler`  

A block that the HealthKit store calls after it finishes executing the query.

This block takes the following parameters:

`query`  
A reference to the query that called this block.

`results`  
An array containing the samples that the query found, or `nil` if an error occurs.

`error`  
If an error occurs, an object describing the error; otherwise, it’s `nil`.

## Discussion

Use this initializer to create a sample query for data that matches any of the HKQueryDescriptor objects. Each descriptor can specify a different data type. The system sorts the results by the provided sort descriptors.

After instantiating the query, call the HKHealthStore class’s execute(_:) method to run this query. Queries run on an anonymous background queue. As soon as the query is complete, the system executes the results handler on the background queue, returning samples that match any of the descriptors. You typically dispatch these results to the main queue to update the user interface.

For example, the following code returns all the step count and push count samples sorted based on their start dates:

```
// Create the data types.
let stepCountType = HKQuantityType(.stepCount)
let pushCountType = HKQuantityType(.pushCount)

// Specify the desired sample types.
let stepDescriptor = HKQueryDescriptor(sampleType: stepCountType, predicate: nil)
let pushDescriptor = HKQueryDescriptor(sampleType: pushCountType, predicate: nil)

// Specify the sort descriptors.
let startDateDescriptor = NSSortDescriptor(key: HKSampleSortIdentifierStartDate,
                                           ascending: true)

// Create the query.
let query = HKSampleQuery(queryDescriptors: [stepDescriptor, pushDescriptor],
                           limit: HKObjectQueryNoLimit,
                           sortDescriptors: [startDateDescriptor])  { (query, samples, error) in

    if let error = error {
        // Handle errors here.
    }

    DispatchQueue.main.async {
        // Process the samples here.
    }
}

// Run the query.
store.execute(query)
```

## See Also

### Creating Sample Queries

Executing Sample Queries

Create, run, and sort sample queries.

init(sampleType: HKSampleType, predicate: NSPredicate?, limit: Int, sortDescriptors: [NSSortDescriptor]?, resultsHandler: (HKSampleQuery, [HKSample]?, (any Error)?) -> Void)

Instantiates and returns a sample query.

init(queryDescriptors: [HKQueryDescriptor], limit: Int, resultsHandler: (HKSampleQuery, [HKSample]?, (any Error)?) -> Void)

Creates a query for samples that match any of the descriptors you provided.

let HKObjectQueryNoLimit: Int

A value indicating that the query returns all the matching samples in the HealthKit store.

HealthKit sort descriptors

Identifiers for sorting results.

