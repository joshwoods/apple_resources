

- Core Bluetooth
- CBPeripheralManagerDelegate
-  peripheralManager(\_:central:didUnsubscribeFrom:) 

Instance Method

# peripheralManager(\_:central:didUnsubscribeFrom:)

Tells the delegate that a remote central device unsubscribed from a characteristic’s value.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func peripheralManager(
    _ peripheral: CBPeripheralManager,
    central: CBCentral,
    didUnsubscribeFrom characteristic: CBCharacteristic
)
```

## Parameters 

`peripheral`  

The peripheral manager connected to the remote central.

`central`  

The remote central device that subscribed to the characteristic’s value.

`characteristic`  

The characteristic unsubscribed from.

## Discussion

Core Bluetooth calls this method when a remote central device unsubscribes from the value of one of the local peripheral’s characteristics, by disabling notifications or indications on the characteristic’s value. When called, stop sending the subscribed central updates of updates to the characteristic’s value.

## See Also

### Monitoring Subscriptions to Characteristic Values

func peripheralManager(CBPeripheralManager, central: CBCentral, didSubscribeTo: CBCharacteristic)

Tells the delegate that a remote central device subscribed to a characteristic’s value.

func peripheralManagerIsReady(toUpdateSubscribers: CBPeripheralManager)

Tells the delegate that a local peripheral device is ready to send characteristic value updates.

