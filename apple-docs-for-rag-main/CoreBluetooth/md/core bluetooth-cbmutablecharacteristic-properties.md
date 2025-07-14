

- Core Bluetooth
- CBMutableCharacteristic
-  properties 

Instance Property

# properties

The properties of the characteristic.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var properties: CBCharacteristicProperties { get set }
```

## Discussion

The properties of a characteristic determine the access to and use of the characteristic’s value and descriptors. For a list of the possible values representing the properties of a characteristic, see the CBCharacteristicProperties enumeration in CBCharacteristic. However, you can’t use the broadcast and extendedProperties characteristic properties when creating a mutable characteristic.

## See Also

### Managing a Mutable Characteristic

var value: Data?

The value of the characteristic.

var descriptors: [CBDescriptor]?

An array of the characteristic’s descriptors.

var permissions: CBAttributePermissions

The permissions of the characteristic value.

struct CBAttributePermissions

Values that represent the read, write, and encryption permissions for a characteristic’s value.

var subscribedCentrals: [CBCentral]?

A list of centrals that are currently subscribed to the characteristic’s value.

