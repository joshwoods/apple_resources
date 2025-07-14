

- Core Bluetooth
- CBPeripheral
-  writeValue(\_:for:type:) 

Instance Method

# writeValue(\_:for:type:)

Writes the value of a characteristic.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func writeValue(
    _ data: Data,
    for characteristic: CBCharacteristic,
    type: CBCharacteristicWriteType
)
```

## Parameters 

`data`  

The value to write.

`characteristic`  

The characteristic containing the value to write.

`type`  

The type of write to execute. For a list of the possible types of writes to a characteristic’s value, see CBCharacteristicWriteType.

## Discussion

When you call this method to write the value of a characteristic, the peripheral calls the peripheral(_:didWriteValueFor:error:) method of its delegate object only if you specified the write type as CBCharacteristicWriteType.withResponse. The response you receive through the peripheral(_:didWriteValueFor:error:) delegate method indicates whether the write was successful; if the write failed, it details the cause of the failure in an error.

On the other hand, if you specify the write type as CBCharacteristicWriteType.withoutResponse, Core Bluetooth attempts to write the value but doesn’t guarantee success. If the write doesn’t succeed in this case, you aren’t notified and you don’t receive an error indicating the cause of the failure.

Use the write and writeWithoutResponse members of the characteristic’s properties enumeration to determine which kinds of writes you can perform.

This method copies the data passed into the `data` parameter, and you can dispose of it after the method returns.

## See Also

### Writing Characteristic and Descriptor Values

func writeValue(Data, for: CBDescriptor)

Writes the value of a characteristic descriptor.

func maximumWriteValueLength(for: CBCharacteristicWriteType) -> Int

The maximum amount of data, in bytes, you can send to a characteristic in a single write type.

enum CBCharacteristicWriteType

Values representing the possible write types to a characteristic’s value.

