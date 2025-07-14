

- Core Bluetooth
- CBPeripheralDelegate
-  peripheral(\_:didDiscoverDescriptorsFor:error:) 

Instance Method

# peripheral(\_:didDiscoverDescriptorsFor:error:)

Tells the delegate that the peripheral found descriptors for a characteristic.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func peripheral(
    _ peripheral: CBPeripheral,
    didDiscoverDescriptorsFor characteristic: CBCharacteristic,
    error: (any Error)?
)
```

## Parameters 

`peripheral`  

The peripheral providing this information.

`characteristic`  

The characteristic to which the characteristic descriptors belong.

`error`  

The reason the call failed, or `nil` if no error occurred.

## Discussion

Core Bluetooth invokes this method when your app calls the discoverDescriptors(for:) method. If the peripheral successfully discovers the descriptors of the specified characteristic, you can access them through the characteristic’s descriptors property. If successful, the `error` parameter is `nil`. If unsuccessful, the `error` parameter returns the cause of the failure.

## See Also

### Discovering Characteristics and their Descriptors

func peripheral(CBPeripheral, didDiscoverCharacteristicsFor: CBService, error: (any Error)?)

Tells the delegate that the peripheral found characteristics for a service.

