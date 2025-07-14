

- HomeKit
- HMCharacteristic
-  isNotificationEnabled 

Instance Property

# isNotificationEnabled

A Boolean indicating whether the characteristic has been set to send notifications.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var isNotificationEnabled: Bool { get }
```

## Discussion

HomeKit delivers notifications to the accessory delegate using the accessory(_:service:didUpdateValueFor:) method.

## See Also

### Receiving change notifications

func enableNotification(Bool, completionHandler: ((any Error)?) -> Void)

Enables or disables notifications for changes in the value of the characteristic.

