

- HealthKit
-  HKObserverQueryCompletionHandler 

Type Alias

# HKObserverQueryCompletionHandler

The completion handler for background deliveries.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
typealias HKObserverQueryCompletionHandler = () -> Void
```

## Mentioned in 

Executing Observer Queries

## Discussion

This completion handler defines a block that can be called when responding to background deliveries. If your app registers for background deliveries, HealthKit wakes your app when new data has been saved to the HealthKit store. You can specify a maximum frequency for background deliveries. HealthKit wakes your app only once during each time period that is defined by the frequency.

When HealthKit wakes your app, it calls the update handler on any observer queries that match the new data. This block is passed to the update handler. You must call this block as soon as you are done processing the incoming data. Calling this block tells HealthKit that you have successfully received the background data. If you do not call this block, HealthKit continues to attempt to launch your app using a back off algorithm. If your app fails to respond three times, HealthKit assumes that your app cannot receive data, and stops sending you background updates.

## See Also

### Related Documentation

func enableBackgroundDelivery(for: HKObjectType, frequency: HKUpdateFrequency, withCompletion: (Bool, (any Error)?) -> Void)

Enables the delivery of updates to an app running in the background.

### Creating Observer Queries

Executing Observer Queries

Create and run observer queries.

init(sampleType: HKSampleType, predicate: NSPredicate?, updateHandler: (HKObserverQuery, HKObserverQueryCompletionHandler, (any Error)?) -> Void)

Instantiates and returns a query that monitors the HealthKit store and responds to changes.

init(queryDescriptors: [HKQueryDescriptor], updateHandler: (HKObserverQuery, Set&lt;HKSampleType>?, HKObserverQueryCompletionHandler, (any Error)?) -> Void)

Creates a query that monitors the HealthKit store and responds to any changes matching any of the query descriptors you provided.

