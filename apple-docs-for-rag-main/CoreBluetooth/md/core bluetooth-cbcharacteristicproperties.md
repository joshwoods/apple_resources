

- Core Bluetooth
-  CBCharacteristicProperties 

Structure

# CBCharacteristicProperties

Values that represent the possible properties of a characteristic.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
struct CBCharacteristicProperties
```

## Overview

Since you can combine characteristic properties, a characteristic may have multiple property values set.

## Topics

### Creating a Characteristic Properties Instance

init(rawValue: UInt)

Creates a characteristic properties instance from the given raw value.

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

static var indicateEncryptionRequired: CBCharacteristicProperties

A property that indicates only trusted devices can enable indications of the characteristic’s value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Accessing Characteristic Data

var value: Data?

The value of the characteristic.

var descriptors: [CBDescriptor]?

A list of the descriptors discovered in this characteristic.

var properties: CBCharacteristicProperties

The properties of the characteristic.

var isNotifying: Bool

A Boolean value that indicates whether the characteristic is currently notifying a subscribed central of its value.

var isBroadcasted: Bool

A Boolean value that indicates whether the characteristic the service broadcasts this characteristic.

