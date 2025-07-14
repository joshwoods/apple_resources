

- Core Bluetooth
- CBPeripheral
-  readRSSI() 

Instance Method

# readRSSI()

Retrieves the current RSSI value for the peripheral while connected to the central manager.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func readRSSI()
```

## Discussion

On macOS, when you call this method to retrieve the Received Signal Strength Indicator (RSSI) of the peripheral while connected to the central manager, the peripheral calls the peripheralDidUpdateRSSI(_:error:) method of its delegate object. If retrieving the RSSI value of the peripheral succeeds, you can access it through the peripheral’s rssi property.

On iOS and tvOS, when you call this method to retrieve the RSSI of the peripheral while connected to the central manager, the peripheral calls the peripheral(_:didReadRSSI:error:) method of its delegate object, which includes the RSSI value as a parameter.

## See Also

### Accessing a Peripheral’s Signal Strength

var rssi: NSNumber?

The Received Signal Strength Indicator (RSSI), in decibels, of the peripheral.

Deprecated

