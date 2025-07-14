

- Core Bluetooth
- CBPeripheral
-  maximumWriteValueLength(for:) 

Instance Method

# maximumWriteValueLength(for:)

The maximum amount of data, in bytes, you can send to a characteristic in a single write type.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func maximumWriteValueLength(for type: CBCharacteristicWriteType) -> Int
```

## Parameters 

`type`  

The characteristic write type to inspect.

## See Also

### Writing Characteristic and Descriptor Values

func writeValue(Data, for: CBCharacteristic, type: CBCharacteristicWriteType)

Writes the value of a characteristic.

func writeValue(Data, for: CBDescriptor)

Writes the value of a characteristic descriptor.

enum CBCharacteristicWriteType

Values representing the possible write types to a characteristic’s value.

