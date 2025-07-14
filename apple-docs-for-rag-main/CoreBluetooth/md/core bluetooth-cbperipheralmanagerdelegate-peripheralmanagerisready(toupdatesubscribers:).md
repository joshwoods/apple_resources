

- Core Bluetooth
- CBPeripheralManagerDelegate
-  peripheralManagerIsReady(toUpdateSubscribers:) 

Instance Method

# peripheralManagerIsReady(toUpdateSubscribers:)

Tells the delegate that a local peripheral device is ready to send characteristic value updates.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func peripheralManagerIsReady(toUpdateSubscribers peripheral: CBPeripheralManager)
```

## Parameters 

`peripheral`  

The peripheral manager that sends characteristic value updates.

## Discussion

When a call to the updateValue(_:for:onSubscribedCentrals:) method fails because the underlying queue used to transmit the updated characteristic value is full, Core Bluetooth calls the peripheralManagerIsReady(toUpdateSubscribers:) method when more space in the transmit queue becomes available. You can then implement this delegate method to resend the value.

## See Also

### Monitoring Subscriptions to Characteristic Values

func peripheralManager(CBPeripheralManager, central: CBCentral, didSubscribeTo: CBCharacteristic)

Tells the delegate that a remote central device subscribed to a characteristic’s value.

func peripheralManager(CBPeripheralManager, central: CBCentral, didUnsubscribeFrom: CBCharacteristic)

Tells the delegate that a remote central device unsubscribed from a characteristic’s value.

