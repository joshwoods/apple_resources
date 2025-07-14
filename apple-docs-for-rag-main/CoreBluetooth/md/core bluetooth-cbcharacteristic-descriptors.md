

- Core Bluetooth
- CBCharacteristic
-  descriptors 

Instance Property

# descriptors

A list of the descriptors discovered in this characteristic.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var descriptors: [CBDescriptor]? { get }
```

## Discussion

The value of this property is an array of CBDescriptor objects that represent a characteristic’s descriptors. Characteristic descriptors provide more information about a characteristic’s value. For example, they may describe the value in human-readable form and describe how to format the value for presentation purposes. For more information about characteristic descriptors, see CBDescriptor.

## See Also

### Accessing Characteristic Data

var value: Data?

The value of the characteristic.

var properties: CBCharacteristicProperties

The properties of the characteristic.

struct CBCharacteristicProperties

Values that represent the possible properties of a characteristic.

var isNotifying: Bool

A Boolean value that indicates whether the characteristic is currently notifying a subscribed central of its value.

var isBroadcasted: Bool

A Boolean value that indicates whether the characteristic the service broadcasts this characteristic.

