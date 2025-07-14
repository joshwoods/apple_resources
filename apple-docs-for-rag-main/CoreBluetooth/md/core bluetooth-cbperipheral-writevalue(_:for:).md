

- Core Bluetooth
- CBPeripheral
-  writeValue(\_:for:) 

Instance Method

# writeValue(\_:for:)

Writes the value of a characteristic descriptor.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func writeValue(
    _ data: Data,
    for descriptor: CBDescriptor
)
```

## Parameters 

`data`  

The value to write.

`descriptor`  

The descriptor containing the value to write.

## Discussion

When you call this method to write the value of a characteristic descriptor, the peripheral calls the peripheral(_:didWriteValueFor:error:) method of its delegate object.

This method copies the `data` passed into the data parameter, and you can dispose of it after the method returns.

You can’t use this method to write the value of a client configuration descriptor (represented by the CBUUIDClientCharacteristicConfigurationString constant), which describes the configuration of notification or indications for a characteristic’s value. If you want to manage notifications or indications for a characteristic’s value, you must use the setNotifyValue(_:for:) method instead.

## See Also

### Writing Characteristic and Descriptor Values

func writeValue(Data, for: CBCharacteristic, type: CBCharacteristicWriteType)

Writes the value of a characteristic.

func maximumWriteValueLength(for: CBCharacteristicWriteType) -> Int

The maximum amount of data, in bytes, you can send to a characteristic in a single write type.

enum CBCharacteristicWriteType

Values representing the possible write types to a characteristic’s value.

