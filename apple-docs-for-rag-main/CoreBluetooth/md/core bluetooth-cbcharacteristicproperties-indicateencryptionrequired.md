

- Core Bluetooth
- CBCharacteristicProperties
-  indicateEncryptionRequired 

Type Property

# indicateEncryptionRequired

A property that indicates only trusted devices can enable indications of the characteristic’s value.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var indicateEncryptionRequired: CBCharacteristicProperties { get }
```

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

static var authenticatedSignedWrites: CBCharacteristicProperties

A property that indicates the perhipheral allows signed writes of the characteristic’s value, without a response to indicate the write succeeded.

static var extendedProperties: CBCharacteristicProperties

A property that indicates the characteristic defines additional properties in the extended properties descriptor.

static var notifyEncryptionRequired: CBCharacteristicProperties

A property that indicates that only trusted devices can enable notifications of the characteristic’s value.

