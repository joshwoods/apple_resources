

- HomeKit
- HMCharacteristic
-  enableNotification(\_:completionHandler:) 

Instance Method

# enableNotification(\_:completionHandler:)

Enables or disables notifications for changes in the value of the characteristic.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
func enableNotification(
    _ enable: Bool,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func enableNotification(_ enable: Bool) async throws
```

## Parameters 

`enable`  

true to enable notifications, false to disable notifications.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## Discussion

HomeKit delivers notifications to the accessory delegate using the accessory(_:service:didUpdateValueFor:) method.

## See Also

### Receiving change notifications

var isNotificationEnabled: Bool

A Boolean indicating whether the characteristic has been set to send notifications.

