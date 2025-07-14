

- Core Bluetooth
- CBPeripheralManager
-  updateValue(\_:for:onSubscribedCentrals:) 

Instance Method

# updateValue(\_:for:onSubscribedCentrals:)

Send an updated characteristic value to one or more subscribed centrals, using a notification or indication.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func updateValue(
    _ value: Data,
    for characteristic: CBMutableCharacteristic,
    onSubscribedCentrals centrals: [CBCentral]?
) -> Bool
```

## Parameters 

`value`  

The characteristic value you want to send via a notification or indication.

`characteristic`  

The characteristic whose value has changed.

`centrals`  

A list of centrals (represented by CBCentral objects) that have subscribed to receive updates of the characteristic’s value. If `nil`, the manager updates all subscribed centrals. The manager ignores any centrals that haven’t subscribed to the characteristic’s value.

## Return Value

This value is true if the update is successfully sent to the subscribed central or centrals. false if the update isn’t successfully sent because the underlying transmit queue is full.

## Discussion

You use this method to send updates of a characteristic’s value—through a notification or indication—to selected centrals that have subscribed to that characteristic’s value. If the method returns false because the underlying transmit queue is full, the peripheral manager calls the peripheralManagerIsReady(toUpdateSubscribers:) method of its delegate object when more space in the transmit queue becomes available. After you receive this delegate method callback, you may resend the update.

If the length of the `value` parameter exceeds the length of the maximumUpdateValueLength property of a subscribed CBCentral, the `value` parameter truncates accordingly.

