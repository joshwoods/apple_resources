

- Core Bluetooth
- CBCharacteristic
-  isNotifying 

Instance Property

# isNotifying

A Boolean value that indicates whether the characteristic is currently notifying a subscribed central of its value.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isNotifying: Bool { get }
```

## Discussion

This value is true if you enabled notifications or indications for the characteristic by successfully calling the setNotifyValue(_:for:) method of the CBPeripheral class. In this case, the peripheral updates its connected central that whenever the characteristic’s value changes.

If the value of the property is false, notifications (or indications) aren’t enabled for the characteristic, and the peripheral doesn’t update its connected central when the characteristic’s value changes.

## Topics

### Related Documentation

func setNotifyValue(Bool, for: CBCharacteristic)

Sets notifications or indications for the value of a specified characteristic.

## See Also

### Accessing Characteristic Data

var value: Data?

The value of the characteristic.

var descriptors: [CBDescriptor]?

A list of the descriptors discovered in this characteristic.

var properties: CBCharacteristicProperties

The properties of the characteristic.

struct CBCharacteristicProperties

Values that represent the possible properties of a characteristic.

var isBroadcasted: Bool

A Boolean value that indicates whether the characteristic the service broadcasts this characteristic.

