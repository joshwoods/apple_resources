

- HealthKit
- HKHealthStore
-  disableBackgroundDelivery(for:withCompletion:) 

Instance Method

# disableBackgroundDelivery(for:withCompletion:)

Disables background deliveries of update notifications for the specified data type.

iOSiPadOSMac Catalyst 13.0+macOS 13.0+visionOSwatchOS 8.0+

``` source
func disableBackgroundDelivery(
    for type: HKObjectType,
    withCompletion completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func disableBackgroundDelivery(for type: HKObjectType) async throws
```

## Parameters 

`type`  

The type of data. This object can be any concrete subclass of the HKObjectType class (any of the classes HKCharacteristicType , HKQuantityType, HKCategoryType, HKWorkoutType or HKCorrelationType).

`completion`  

A block that this method calls as soon as the background delivery is disabled. This block is passed the following parameters:

success  
A Boolean value. This parameter contains true if the background delivery was successfully disabled; otherwise, false.

error  
An error object. If an error occurred, this object contains information about the error; otherwise, it is set to `nil`.

## Discussion

Call this method to prevent your app from receiving any additional update notifications about the specified data type while in the background. This method operates asynchronously. As soon as the background delivery is disabled, this method calls its completion handler on a background queue.

## See Also

### Related Documentation

class HKObserverQuery

A long-running query that monitors the HealthKit store and updates your app when the HealthKit store saves or deletes a matching sample.

### Managing background delivery

func enableBackgroundDelivery(for: HKObjectType, frequency: HKUpdateFrequency, withCompletion: (Bool, (any Error)?) -> Void)

Enables the delivery of updates to an app running in the background.

com.apple.developer.healthkit.background-delivery

A Boolean value that indicates whether observer queries receive updates while running in the background.

enum HKUpdateFrequency

Constants that determine how often the system launches your app in response to changes to HealthKit data.

func disableAllBackgroundDelivery(completion: (Bool, (any Error)?) -> Void)

Disables all background deliveries of update notifications.

