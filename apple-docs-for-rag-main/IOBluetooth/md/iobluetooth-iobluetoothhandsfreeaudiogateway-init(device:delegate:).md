

- IOBluetooth
- IOBluetoothHandsFreeAudioGateway
-  init(device:delegate:) 

Initializer

# init(device:delegate:)

Creates an object that controls a connected Bluetooth hands-free phone or headset.

macOS 10.7+

``` source
init!(
    device: IOBluetoothDevice!,
    delegate inDelegate: Any!
)
```

## Parameters 

`device`  

A remote Bluetooth phone or headset.

`inDelegate`  

A delegate that conforms to the IOBluetoothHandsFreeAudioGatewayDelegate protocol.

