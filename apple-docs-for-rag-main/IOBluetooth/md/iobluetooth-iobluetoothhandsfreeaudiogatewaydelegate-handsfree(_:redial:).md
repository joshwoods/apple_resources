

- IOBluetooth
- IOBluetoothHandsFreeAudioGatewayDelegate
-  handsFree(\_:redial:) 

Instance Method

# handsFree(\_:redial:)

Tells the delegate the connected Bluetooth hands-free phone or headset is redialing the last phone number.

macOS 10.7+

``` source
optional func handsFree(
    _ device: IOBluetoothHandsFreeAudioGateway!,
    redial: NSNumber!
)
```

## Parameters 

`device`  

The audio gateway for the remote hands-free Bluetooth device.

`redial`  

A number that indicates whether the device is attempting to redial. This value is always set to 1.

## See Also

### Receiving Status Change Information

func handsFree(IOBluetoothHandsFreeAudioGateway!, hangup: NSNumber!)

Tells the delegate the connected Bluetooth hands-free phone or headset is sending a hang-up signal.

