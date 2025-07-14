

- Core Bluetooth
- CBPeripheral
-  discoverDescriptors(for:) 

Instance Method

# discoverDescriptors(for:)

Discovers the descriptors of a characteristic.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func discoverDescriptors(for characteristic: CBCharacteristic)
```

## Parameters 

`characteristic`  

The characteristic whose descriptors you want to discover.

## Discussion

When the peripheral discovers one or more descriptors of the specified characteristic, it calls the peripheral(_:didDiscoverDescriptorsFor:error:) method of its delegate object. After the peripheral discovers the descriptors of the characteristic, you can access them through the characteristic’s descriptors property.

## See Also

### Discovering Characteristics and Descriptors

func discoverCharacteristics([CBUUID]?, for: CBService)

Discovers the specified characteristics of a service.

