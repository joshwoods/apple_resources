

- Core Bluetooth
- CBPeripheralDelegate
-  peripheralDidUpdateRSSI(\_:error:) Deprecated

Instance Method

# peripheralDidUpdateRSSI(\_:error:)

Tells the delegate that retrieving the value of the peripheral’s current Received Signal Strength Indicator (RSSI) succeeded.

iOS 5.0–8.0DeprecatediPadOS 5.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.13DeprecatedtvOS 9.0+visionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
optional func peripheralDidUpdateRSSI(
    _ peripheral: CBPeripheral,
    error: (any Error)?
)
```

Deprecated

in iOS and tvOS, use the peripheral(_:didReadRSSI:error:) method instead.

## Parameters 

`peripheral`  

The peripheral providing this information.

`error`  

The reason the call failed, or `nil` if no error occurred.

## Discussion

Core Bluetooth invokes this method when your app calls the readRSSI() method, while the peripheral is connected to the central manager. If successful, the `error` parameter is `nil`. If unsuccessful, the `error` parameter returns the cause of the failure.

## See Also

### Retrieving a Peripheral’s RSSI Data

func peripheral(CBPeripheral, didReadRSSI: NSNumber, error: (any Error)?)

Tells the delegate that retrieving the value of the peripheral’s current Received Signal Strength Indicator (RSSI) succeeded.

