

- Core Bluetooth
- CBPeripheralDelegate
-  peripheralIsReady(toSendWriteWithoutResponse:) 

Instance Method

# peripheralIsReady(toSendWriteWithoutResponse:)

Tells the delegate that a peripheral is again ready to send characteristic updates.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func peripheralIsReady(toSendWriteWithoutResponse peripheral: CBPeripheral)
```

## Parameters 

`peripheral`  

The peripheral providing this update.

## Discussion

The peripheral calls this delegate method after a failed call to writeValue(_:for:type:), once `peripheral` is ready to send characteristic value updates.

## See Also

### Writing Characteristic and Descriptor Values

func peripheral(CBPeripheral, didWriteValueFor: CBCharacteristic, error: (any Error)?)

Tells the delegate that the peripheral successfully set a value for the characteristic.

func peripheral(CBPeripheral, didWriteValueFor: CBDescriptor, error: (any Error)?)

Tells the delegate that the peripheral successfully set a value for the descriptor.

