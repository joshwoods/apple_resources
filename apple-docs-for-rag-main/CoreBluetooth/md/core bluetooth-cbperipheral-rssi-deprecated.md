

- Core Bluetooth
- CBPeripheral
-  rssi Deprecated

Instance Property

# rssi

The Received Signal Strength Indicator (RSSI), in decibels, of the peripheral.

iOS 5.0–8.0DeprecatediPadOS 5.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.13DeprecatedtvOS 9.0+visionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
var rssi: NSNumber? { get }
```

Deprecated

On iOS and tvOS, when you call the readRSSI() method, the system returns the RSSI as a parameter in a call to the delegate’s peripheral(_:didReadRSSI:error:) method. Use that value instead.

## Discussion

Returns a number, in decibels, that indicates the RSSI of the peripheral while connected to the central manager. You can use a connected peripheral’s RSSI property to determine the peripheral’s proximity. The default value of this property is `nil`; the first successful call to readRSSI() sets its value.

## See Also

### Accessing a Peripheral’s Signal Strength

func readRSSI()

Retrieves the current RSSI value for the peripheral while connected to the central manager.

