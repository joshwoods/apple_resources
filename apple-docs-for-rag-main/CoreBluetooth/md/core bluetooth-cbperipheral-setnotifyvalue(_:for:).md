

- Core Bluetooth
- CBPeripheral
-  setNotifyValue(\_:for:) 

Instance Method

# setNotifyValue(\_:for:)

Sets notifications or indications for the value of a specified characteristic.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setNotifyValue(
    _ enabled: Bool,
    for characteristic: CBCharacteristic
)
```

## Parameters 

`enabled`  

A Boolean value that indicates whether to receive notifications or indications whenever the characteristic’s value changes. true if you want to enable notifications or indications for the characteristic’s value. false if you don’t want to receive notifications or indications whenever the characteristic’s value changes.

`characteristic`  

The specified characteristic.

## Discussion

When you enable notifications for the characteristic’s value, the peripheral calls the peripheral(_:didUpdateNotificationStateFor:error:) method of its delegate object to indicate if the action succeeded. If successful, the peripheral then calls the peripheral(_:didUpdateValueFor:error:) method of its delegate object whenever the characteristic value changes. Because the peripheral chooses when it sends an update, your app should prepare to handle them as long as notifications or indications remain enabled. If the specified characteristic’s configuration allows both notifications and indications, calling this method enables notifications only. You can disable notifications and indications for a characteristic’s value by calling this method with the `enabled` parameter set to false.

## Topics

### Related Documentation

let CBConnectPeripheralOptionNotifyOnNotificationKey: String

A Boolean value that specifies whether the system should display an alert for any notification sent by a peripheral.

