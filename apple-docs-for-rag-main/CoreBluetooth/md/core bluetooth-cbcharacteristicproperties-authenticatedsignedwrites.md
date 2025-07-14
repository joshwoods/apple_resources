

- Core Bluetooth
- CBCharacteristicProperties
-  authenticatedSignedWrites 

Type Property

# authenticatedSignedWrites

A property that indicates the perhipheral allows signed writes of the characteristic’s value, without a response to indicate the write succeeded.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
static var authenticatedSignedWrites: CBCharacteristicProperties { get }
```

## Discussion

If a characteristic has this property set, it returns an error to the central when it fails to write the characteristic’s value.

## See Also

### Characteristic Properties

static var broadcast: CBCharacteristicProperties

A property that indicates the characteristic can broadcast its value using a characteristic configuration descriptor.

static var read: CBCharacteristicProperties

A property that indicates a peripheral can read the characteristic’s value.

static var writeWithoutResponse: CBCharacteristicProperties

A property that indicates a peripheral can write the characteristic’s value, without a response to indicate that the write succeeded.

static var write: CBCharacteristicProperties

A property that indicates a peripheral can write the characteristic’s value, with a response to indicate that the write succeeded.

static var notify: CBCharacteristicProperties

A property that indicates the peripheral permits notifications of the characteristic’s value, without a response from the central to indicate receipt of the notification.

static var indicate: CBCharacteristicProperties

A property that indicates the peripheral permits notifications of the characteristic’s value, with a response from the central to indicate receipt of the notification.

static var extendedProperties: CBCharacteristicProperties

A property that indicates the characteristic defines additional properties in the extended properties descriptor.

static var notifyEncryptionRequired: CBCharacteristicProperties

A property that indicates that only trusted devices can enable notifications of the characteristic’s value.

static var indicateEncryptionRequired: CBCharacteristicProperties

A property that indicates only trusted devices can enable indications of the characteristic’s value.

