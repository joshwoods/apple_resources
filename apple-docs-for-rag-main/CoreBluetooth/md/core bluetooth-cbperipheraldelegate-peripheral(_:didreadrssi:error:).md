

- Core Bluetooth
- CBPeripheralDelegate
-  peripheral(\_:didReadRSSI:error:) 

Instance Method

# peripheral(\_:didReadRSSI:error:)

Tells the delegate that retrieving the value of the peripheral’s current Received Signal Strength Indicator (RSSI) succeeded.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.13+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func peripheral(
    _ peripheral: CBPeripheral,
    didReadRSSI RSSI: NSNumber,
    error: (any Error)?
)
```

## Parameters 

`peripheral`  

The peripheral providing this information.

`RSSI`  

The RSSI, in decibels, of the peripheral.

`error`  

The reason the call failed, or `nil` if no error occurred.

## Discussion

Core Bluetooth invokes this method when your app calls the readRSSI() method, while the peripheral is connected to the central manager. If successful, the `error` parameter is `nil` and the parameter `RSSI` reports the peripheral’s signal strength, in decibels. If unsuccessful, the `error` parameter returns the cause of the failure.

## See Also

### Retrieving a Peripheral’s RSSI Data

func peripheralDidUpdateRSSI(CBPeripheral, error: (any Error)?)

Tells the delegate that retrieving the value of the peripheral’s current Received Signal Strength Indicator (RSSI) succeeded.

Deprecated

