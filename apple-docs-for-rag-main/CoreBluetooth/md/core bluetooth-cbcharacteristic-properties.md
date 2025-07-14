

- Core Bluetooth
- CBCharacteristic
-  properties 

Instance Property

# properties

The properties of the characteristic.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var properties: CBCharacteristicProperties { get }
```

## Discussion

The properties of a characteristic determine the access to and use of the characteristic’s value and descriptors. For a list of the possible values representing the properties of a characteristic, see CBCharacteristicProperties.

## See Also

### Accessing Characteristic Data

var value: Data?

The value of the characteristic.

var descriptors: [CBDescriptor]?

A list of the descriptors discovered in this characteristic.

struct CBCharacteristicProperties

Values that represent the possible properties of a characteristic.

var isNotifying: Bool

A Boolean value that indicates whether the characteristic is currently notifying a subscribed central of its value.

var isBroadcasted: Bool

A Boolean value that indicates whether the characteristic the service broadcasts this characteristic.

