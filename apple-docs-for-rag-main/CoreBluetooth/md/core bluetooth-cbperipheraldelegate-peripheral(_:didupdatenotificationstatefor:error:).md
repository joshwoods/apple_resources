

- Core Bluetooth
- CBPeripheralDelegate
-  peripheral(\_:didUpdateNotificationStateFor:error:) 

Instance Method

# peripheral(\_:didUpdateNotificationStateFor:error:)

Tells the delegate that the peripheral received a request to start or stop providing notifications for a specified characteristic’s value.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func peripheral(
    _ peripheral: CBPeripheral,
    didUpdateNotificationStateFor characteristic: CBCharacteristic,
    error: (any Error)?
)
```

## Parameters 

`peripheral`  

The peripheral providing this information.

`characteristic`  

The characteristic for which to configure value notifications.

`error`  

The reason the call failed, or `nil` if no error occurred.

## Discussion

Core Bluetooth invokes this method when your app calls the setNotifyValue(_:for:) method. If successful, the `error` parameter is `nil`. If unsuccessful, the `error` parameter returns the cause of the failure.

