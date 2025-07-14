

- HealthKit
- Queries
- HKObserverQuery
-  Executing Observer Queries 

Article

# Executing Observer Queries

Create and run observer queries.

## Overview

Observer queries are long-running queries that monitor the HealthKit store on a background thread, and update your app when the HealthKit store saves or deletes a matching sample. By default, observer queries only return results while your app is in the foreground; however, you can configure your app to also receive update notifications in the background.

### Create Observer Queries

To create an observer query, call the init(sampleType:predicate:updateHandler:) initializer. Start by creating a type object for the samples you want to observe. The following example creates a type object for step counts.

```
guard let stepCountType = HKObjectType.quantityType(forIdentifier: .stepCount) else {
    // This should never fail when using a defined constant.
    fatalError("*** Unable to get the step count type ***")
}
```

Next, create the observer query.

```
let query = HKObserverQuery(sampleType: stepCountType, predicate: nil) { (query, completionHandler, errorOrNil) in

    if let error = errorOrNil {
        // Properly handle the error.
        return
    }

    // Take whatever steps are necessary to update your app.
    // This often involves executing other queries to access the new data.

    // If you have subscribed for background updates you must call the completion handler here.
    // completionHandler()
}
```

After the query is instantiated, call the HealthKit store’s execute(_:) method.

```
store.execute(query)
```

This runs the query on an anonymous background queue. Whenever a matching sample is added to or deleted from the HealthKit store, the system calls the query’s update handler on the same background queue (but not necessarily the same thread).

Note

The observer query’s update handler does not receive any information about the change—just that a change occurred. You must execute another query, for example an HKSampleQuery or HKAnchoredObjectQuery, to access the changes.

To stop the query, call the HealthKit store’s stop(_:) method.

### Receive Background Deliveries

Apps can also register to receive updates while in the background by calling the HealthKit store’s enableBackgroundDelivery(for:frequency:withCompletion:) method. This method registers your app for background notifications. HealthKit wakes your app when the store receives new samples of the specified type. HealthKit notifies your app at most once per time period defined by the frequency you specified when registering.

As soon as your app launches, HealthKit calls the update handler for any observer queries that match the newly saved data. If you plan on supporting background delivery, set up all your observer queries in your app delegate’s application(_:didFinishLaunchingWithOptions:) method. By setting up the queries in application(_:didFinishLaunchingWithOptions:), you ensure that the queries are instantiated and ready to use before HealthKit delivers the updates.

After your observer queries have finished processing the new data, you must call the update’s completion handler to notify HealthKit that you have successfully received the background delivery.

Important

Background server queries aren’t supported on the Simulator. Be sure to test your background queries on a device.

For more information on managing background deliveries, see Managing Background Deliveries in HKHealthStore. For more information on the background delivery completion handler, see HKObserverQueryCompletionHandler.

## See Also

### Creating Observer Queries

init(sampleType: HKSampleType, predicate: NSPredicate?, updateHandler: (HKObserverQuery, HKObserverQueryCompletionHandler, (any Error)?) -> Void)

Instantiates and returns a query that monitors the HealthKit store and responds to changes.

init(queryDescriptors: [HKQueryDescriptor], updateHandler: (HKObserverQuery, Set&lt;HKSampleType>?, HKObserverQueryCompletionHandler, (any Error)?) -> Void)

Creates a query that monitors the HealthKit store and responds to any changes matching any of the query descriptors you provided.

typealias HKObserverQueryCompletionHandler

The completion handler for background deliveries.

