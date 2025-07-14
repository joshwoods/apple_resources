

- HealthKit
- HKActivitySummaryQuery
-  init(predicate:resultsHandler:) 

Initializer

# init(predicate:resultsHandler:)

Initializes a new active summary query.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
init(
    predicate: NSPredicate?,
    resultsHandler handler: @escaping (HKActivitySummaryQuery, [HKActivitySummary]?, (any Error)?) -> Void
)
```

## Parameters 

`predicate`  

A predicate that filters the activity summaries returned by the query. Pass `nil` to receive all activity samples.

`handler`  

A block that is called after the initial results have been gathered. This block takes the following parameters:

query  
A reference to the query calling this block.

activitySummaries  
An array containing the summaries returned by this query, or `nil` if an error occurred.

error  
If an error occurs, this parameter contains an object describing the error; otherwise, it is `nil`.

## Return Value

A newly initialized activity summary query.

## Mentioned in 

Executing Activity Summary Queries

## Discussion

After instantiating the query, call the HKHealthStore class’s execute(_:) method to run it. The queries run on an anonymous background queue. As soon as the query is complete, the results handler block is executed on the same background queue (but not necessarily the same thread). You typically dispatch these results to the main queue to update the user interface.

Activity summary queries can also act as long-running queries. If you assign an update handler before you execute the query, the query continues to monitor the HealthKit store after gathering the initial results. The update handler is called on a background queue every time a matching sample is saved or updated in the HealthKit store. You can cancel this query by calling the store’s stop(_:) method.

## See Also

### Creating activity summary queries

Executing Activity Summary Queries

Create and run activity summary queries.

