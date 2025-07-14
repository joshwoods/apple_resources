

- Core Bluetooth
- CBPeripheralDelegate
-  peripheral(\_:didDiscoverCharacteristicsFor:error:) 

Instance Method

# peripheral(\_:didDiscoverCharacteristicsFor:error:)

Tells the delegate that the peripheral found characteristics for a service.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func peripheral(
    _ peripheral: CBPeripheral,
    didDiscoverCharacteristicsFor service: CBService,
    error: (any Error)?
)
```

## Parameters 

`peripheral`  

The peripheral providing this information.

`service`  

The service to which the characteristics belong.

`error`  

The reason the call failed, or `nil` if no error occurred.

## Discussion

Core Bluetooth invokes this method when your app calls the discoverCharacteristics(_:for:) method. If the peripheral successfully discovers the characteristics of the specified service, you can access them through the service’s characteristics property. If successful, the `error` parameter is `nil`. If unsuccessful, the `error` parameter returns the cause of the failure.

## See Also

### Discovering Characteristics and their Descriptors

func peripheral(CBPeripheral, didDiscoverDescriptorsFor: CBCharacteristic, error: (any Error)?)

Tells the delegate that the peripheral found descriptors for a characteristic.

