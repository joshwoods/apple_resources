

- HealthKit
- HKHealthStore
-  disableAllBackgroundDelivery(completion:) 

Instance Method

# disableAllBackgroundDelivery(completion:)

Disables all background deliveries of update notifications.

iOSiPadOSMac Catalyst 13.0+macOS 13.0+visionOSwatchOS 8.0+

``` source
func disableAllBackgroundDelivery(completion: @escaping (Bool, (any Error)?) -> Void)
```

``` source
func disableAllBackgroundDelivery() async throws
```

## Parameters 

`completion`  

A block that this method calls as soon as the background deliveries are disabled. This block is passed the following parameters:

success  
A Boolean value. This parameter contains true if the background deliveries were successfully disabled; otherwise, false.

error  
An error object. If an error occurred, this object contains information about the error; otherwise, it is set to `nil`.

## Discussion

Call this method to prevent your app from receiving any additional update notifications while in the background. This method operates asynchronously. As soon as the background deliveries are disabled, this method calls its completion handler on a background queue.

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

func disableBackgroundDelivery(for: HKObjectType, withCompletion: (Bool, (any Error)?) -> Void)

Disables background deliveries of update notifications for the specified data type.

