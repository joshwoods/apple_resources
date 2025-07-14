

- Core Bluetooth
- CBPeripheral
-  readValue(for:) 

Instance Method

# readValue(for:)

Retrieves the value of a specified characteristic.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func readValue(for characteristic: CBCharacteristic)
```

## Parameters 

`characteristic`  

The characteristic whose value you want to read.

## Discussion

When you call this method to read the value of a characteristic, the peripheral calls the peripheral(_:didUpdateValueFor:error:) method of its delegate object. If the peripheral successfully reads the value of the characteristic, you can access it through the characteristic’s value property.

Not all characteristics have a readable value. You can determine whether a characteristic’s value is readable by accessing the relevant properties of the CBCharacteristicProperties enumeration.

## See Also

### Reading Characteristic and Descriptor Values

func readValue(for: CBDescriptor)

Retrieves the value of a specified characteristic descriptor.

