

- Core Bluetooth
- CBMutableCharacteristic
-  subscribedCentrals 

Instance Property

# subscribedCentrals

A list of centrals that are currently subscribed to the characteristic’s value.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var subscribedCentrals: [CBCentral]? { get }
```

## Discussion

The value of this property is an array of CBCentral objects that currently subscribe to the characteristic’s value. The array is empty if the characteristic isn’t configured to support notifications or indications. Even if the characteristic’s configuration supports notifications or indications, the array is empty if centrals aren’t subscribing to the characteristic’s value.

## Topics

### Related Documentation

func updateValue(Data, for: CBMutableCharacteristic, onSubscribedCentrals: [CBCentral]?) -> Bool

Send an updated characteristic value to one or more subscribed centrals, using a notification or indication.

## See Also

### Managing a Mutable Characteristic

var value: Data?

The value of the characteristic.

var descriptors: [CBDescriptor]?

An array of the characteristic’s descriptors.

var properties: CBCharacteristicProperties

The properties of the characteristic.

var permissions: CBAttributePermissions

The permissions of the characteristic value.

struct CBAttributePermissions

Values that represent the read, write, and encryption permissions for a characteristic’s value.

