

- Core Bluetooth
- CBPeripheral
-  readValue(for:) 

Instance Method

# readValue(for:)

Retrieves the value of a specified characteristic descriptor.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func readValue(for descriptor: CBDescriptor)
```

## Parameters 

`descriptor`  

The characteristic descriptor whose value you want to read.

## Discussion

When you call this method to read the value of a characteristic descriptor, the peripheral calls the peripheral(_:didUpdateValueFor:error:) method of its delegate object. If the peripheral successfully retrieves the value of the characteristic descriptor, you can access it through the characteristic descriptor’s value property.

## See Also

### Reading Characteristic and Descriptor Values

func readValue(for: CBCharacteristic)

Retrieves the value of a specified characteristic.

