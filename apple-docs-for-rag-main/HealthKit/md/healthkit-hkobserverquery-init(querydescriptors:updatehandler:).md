

- HealthKit
- HKObserverQuery
-  init(queryDescriptors:updateHandler:) 

Initializer

# init(queryDescriptors:updateHandler:)

Creates a query that monitors the HealthKit store and responds to any changes matching any of the query descriptors you provided.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    queryDescriptors: [HKQueryDescriptor],
    updateHandler: @escaping (HKObserverQuery, Set?, @escaping HKObserverQueryCompletionHandler, (any Error)?) -> Void
)
```

## Parameters 

`queryDescriptors`  

An array of descriptors that specifies the types of samples the query returns.

`updateHandler`  

A block that the system calls when a matching sample is saved to or deleted from the HealthKit store. This block takes the following parameters:

`query`  
A reference to the query calling this block.

`sampleTypesAdded`  
A list of data types for all of the changed objects.

`completionHandler`  
If you registered for background updates, call this completion handler as soon as you are done processing the incoming data. This handler tells HealthKit that you successfully received the background update. Additionally, call the completion handler only when you use background updates. For more information on using this completion handler, see HKObserverQueryCompletionHandler.

error  
If an error occurs, an object describing the error; otherwise, it’s `nil`.

## Discussion

Use this initializer to create an observer query for changes that match any of the HKQueryDescriptor objects. Each descriptor can specify a different data type.

After instantiating the query, call the HKHealthStore class’s execute(_:) method to run this query. Observer queries are long-running tasks. They continue to run on an anonymous background thread and call their results handler when the system, the user, or any app adds or deletes a matching sample from the HealthKit store. To stop a query, call the HKHealthStore class’s stop(_:) method. You can use Observer queries to receive updates in the background. For more information, see Executing Observer Queries.

The system calls the update handler block you provide every time something saves or deletes samples matching this query from the HealthKit store. You often need to launch other queries from inside this block to get the updated data. In particular, you can use anchored object queries to retrieve the list of new samples added to the store. For more information, see HKAnchoredObjectQuery.

For example, the following code monitors the store and calls the update handler after any relevant changes:

```
// Create the data types.
let stepCountType = HKQuantityType(.stepCount)
let pushCountType = HKQuantityType(.pushCount)

// Specify the desired sample types.
let stepDescriptor = HKQueryDescriptor(sampleType: stepCountType, predicate: nil)
let pushDescriptor = HKQueryDescriptor(sampleType: pushCountType, predicate: nil)

// Create the query.
let observerQuery = HKObserverQuery(queryDescriptors: [stepDescriptor, pushDescriptor])
{ query, updatedSampleTypes, completionHandler, error in

    if let error = error {
        // Handle errors here.
    }

    if let types = updatedSampleTypes {
        let descriptors = types.map { type in
            HKQueryDescriptor(sampleType: type, predicate: nil)
        }

        // Create an inner query to access the changed data.
        let anchorQuery = HKAnchoredObjectQuery(queryDescriptors: descriptors,
                                                anchor: anchor,
                                                limit: HKObjectQueryNoLimit)
        {
            anchorQuery, samples, deleted, newAnchor, error in
            if let error = error {
                // Handle errors here.
            }

            DispatchQueue.main.async {
                // Update the anchor.
                anchor = newAnchor

                // Process the samples and deleted objects here.

                // Call the observer's completion handler.
                completionHandler()
            }
        }

        // Run the inner query.
        store.execute(anchorQuery)
    }
}
```

## See Also

### Creating Observer Queries

Executing Observer Queries

Create and run observer queries.

init(sampleType: HKSampleType, predicate: NSPredicate?, updateHandler: (HKObserverQuery, HKObserverQueryCompletionHandler, (any Error)?) -> Void)

Instantiates and returns a query that monitors the HealthKit store and responds to changes.

typealias HKObserverQueryCompletionHandler

The completion handler for background deliveries.

