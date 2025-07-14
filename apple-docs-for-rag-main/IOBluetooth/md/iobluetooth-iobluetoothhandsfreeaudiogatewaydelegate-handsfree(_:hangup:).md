

- IOBluetooth
- IOBluetoothHandsFreeAudioGatewayDelegate
-  handsFree(\_:hangup:) 

Instance Method

# handsFree(\_:hangup:)

Tells the delegate the connected Bluetooth hands-free phone or headset is sending a hang-up signal.

macOS 10.7+

``` source
optional func handsFree(
    _ device: IOBluetoothHandsFreeAudioGateway!,
    hangup: NSNumber!
)
```

## Parameters 

`device`  

The remote hands-free Bluetooth device that’s sending a hang-up signal.

`hangup`  

A number that indicates whether the device is sending a hang-up signal. This value is always set to 1.

## See Also

### Receiving Status Change Information

func handsFree(IOBluetoothHandsFreeAudioGateway!, redial: NSNumber!)

Tells the delegate the connected Bluetooth hands-free phone or headset is redialing the last phone number.

