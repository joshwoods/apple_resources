

- Core Bluetooth
- CBMutableCharacteristic
-  descriptors 

Instance Property

# descriptors

An array of the characteristic’s descriptors.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var descriptors: [CBDescriptor]? { get set }
```

## Discussion

The value of this property is an array of CBDescriptor objects that provide more information about a characteristic’s value. For example, they may describe the value in human-readable form and describe how to format the value for presentation purposes. For more information about characteristic descriptors, see CBDescriptor.

## See Also

### Managing a Mutable Characteristic

var value: Data?

The value of the characteristic.

var properties: CBCharacteristicProperties

The properties of the characteristic.

var permissions: CBAttributePermissions

The permissions of the characteristic value.

struct CBAttributePermissions

Values that represent the read, write, and encryption permissions for a characteristic’s value.

var subscribedCentrals: [CBCentral]?

A list of centrals that are currently subscribed to the characteristic’s value.

