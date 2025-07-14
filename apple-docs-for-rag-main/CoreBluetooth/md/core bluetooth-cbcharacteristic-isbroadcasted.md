

- Core Bluetooth
- CBCharacteristic
-  isBroadcasted 

Instance Property

# isBroadcasted

A Boolean value that indicates whether the characteristic the service broadcasts this characteristic.

iOS 5.0–8.0DeprecatediPadOS 5.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.13DeprecatedtvOS 9.0+visionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
var isBroadcasted: Bool { get }
```

## Discussion

Don’t use this deprecated property.

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

var isNotifying: Bool

A Boolean value that indicates whether the characteristic is currently notifying a subscribed central of its value.

