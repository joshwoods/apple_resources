

- Core Bluetooth
-  CBCharacteristicWriteType 

Enumeration

# CBCharacteristicWriteType

Values representing the possible write types to a characteristic’s value.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
enum CBCharacteristicWriteType
```

## Overview

Characteristic write types have corresponding restrictions on the length of the data that you can write to a characteristic’s value. For the CBCharacteristicWriteType.withResponse write type’s restrictions, see the Bluetooth 4.0 specification, Volume 3, Part G, Sections 4.9.3–4. For the CBCharacteristicWriteType.withoutResponse write type restrictions, see the Bluetooth 4.0 specification, Volume 3, Part G, Sections 4.9.1–2.

Tip

When you write with a response, you can write a characteristic value that’s longer than permitted when you write without a response.

## Topics

### Write Types

case withResponse

Write a characteristic value, with a response from the peripheral to indicate whether the write was successful.

case withoutResponse

Write a characteristic value, without any response from the peripheral to indicate whether the write was successful.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Writing Characteristic and Descriptor Values

func writeValue(Data, for: CBCharacteristic, type: CBCharacteristicWriteType)

Writes the value of a characteristic.

func writeValue(Data, for: CBDescriptor)

Writes the value of a characteristic descriptor.

func maximumWriteValueLength(for: CBCharacteristicWriteType) -> Int

The maximum amount of data, in bytes, you can send to a characteristic in a single write type.

