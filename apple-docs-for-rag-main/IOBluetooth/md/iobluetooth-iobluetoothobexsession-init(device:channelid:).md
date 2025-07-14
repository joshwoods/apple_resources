

- IOBluetooth
- IOBluetoothOBEXSession
-  init(device:channelID:) 

Initializer

# init(device:channelID:)

Initializes a Bluetooth-based OBEX Session using a Bluetooth device.

macOS

``` source
init!(
    device inDevice: IOBluetoothDevice!,
    channelID inChannelID: BluetoothRFCOMMChannelID
)
```

## Parameters 

`inDevice`  

The bluetooth device on which to open the OBEXSession.

`inChannelID`  

The RFCOMM channel ID to use when opening the connection.

## See Also

### Initializers

init!(incomingRFCOMMChannel: IOBluetoothRFCOMMChannel!, eventSelector: Selector!, selectorTarget: Any!, refCon: UnsafeMutableRawPointer!)

Initializes a Bluetooth-based OBEX Session using an incoming RFCOMM channel.

init!(sdpServiceRecord: IOBluetoothSDPServiceRecord!)

Initializes a Bluetooth-based OBEX Session using an SDP service record.

