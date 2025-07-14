

- Core Bluetooth
- CBPeripheralDelegate
-  peripheral(\_:didUpdateValueFor:error:) 

Instance Method

# peripheral(\_:didUpdateValueFor:error:)

Tells the delegate that retrieving a specified characteristic descriptor’s value succeeded.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func peripheral(
    _ peripheral: CBPeripheral,
    didUpdateValueFor descriptor: CBDescriptor,
    error: (any Error)?
)
```

## Parameters 

`peripheral`  

The peripheral providing this information.

`descriptor`  

The characteristic descriptor containing the value.

`error`  

The reason the call failed, or `nil` if no error occurred.

## Discussion

Core Bluetooth invokes this method when your app calls the readValue(for:) method. If successful, the `error` parameter is `nil`. If unsuccessful, the `error` parameter returns the cause of the failure.

## See Also

### Retrieving Characteristic and Descriptor Values

func peripheral(CBPeripheral, didUpdateValueFor: CBCharacteristic, error: (any Error)?)

Tells the delegate that retrieving the specified characteristic’s value succeeded, or that the characteristic’s value changed.

