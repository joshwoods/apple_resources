

- Core Bluetooth
- CBMutableCharacteristic
-  permissions 

Instance Property

# permissions

The permissions of the characteristic value.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var permissions: CBAttributePermissions { get set }
```

## Discussion

Characteristic permissions represent the read, write, and encryption permissions for a characteristic’s value. For a complete list and discussion of the available characteristic permissions, see CBAttributePermissions.

## See Also

### Managing a Mutable Characteristic

var value: Data?

The value of the characteristic.

var descriptors: [CBDescriptor]?

An array of the characteristic’s descriptors.

var properties: CBCharacteristicProperties

The properties of the characteristic.

struct CBAttributePermissions

Values that represent the read, write, and encryption permissions for a characteristic’s value.

var subscribedCentrals: [CBCentral]?

A list of centrals that are currently subscribed to the characteristic’s value.

