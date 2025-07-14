

- Core Bluetooth
- CBPeripheralDelegate
-  peripheral(\_:didWriteValueFor:error:) 

Instance Method

# peripheral(\_:didWriteValueFor:error:)

Tells the delegate that the peripheral successfully set a value for the characteristic.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func peripheral(
    _ peripheral: CBPeripheral,
    didWriteValueFor characteristic: CBCharacteristic,
    error: (any Error)?
)
```

## Parameters 

`peripheral`  

The peripheral providing this information.

`characteristic`  

The characteristic containing the value.

`error`  

The reason the call failed, or `nil` if no error occurred.

## Discussion

Core Bluetooth invokes this method only when your app calls the writeValue(_:for:type:) method with the CBCharacteristicWriteType.withResponse constant specified as the write type. If successful, the `error` parameter is `nil`. If unsuccessful, the `error` parameter returns the cause of the failure.

## See Also

### Writing Characteristic and Descriptor Values

func peripheral(CBPeripheral, didWriteValueFor: CBDescriptor, error: (any Error)?)

Tells the delegate that the peripheral successfully set a value for the descriptor.

func peripheralIsReady(toSendWriteWithoutResponse: CBPeripheral)

Tells the delegate that a peripheral is again ready to send characteristic updates.

