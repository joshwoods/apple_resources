

- IOBluetooth
- IOBluetoothOBEXSession
-  init(sdpServiceRecord:) 

Initializer

# init(sdpServiceRecord:)

Initializes a Bluetooth-based OBEX Session using an SDP service record.

macOS

``` source
init!(sdpServiceRecord inSDPServiceRecord: IOBluetoothSDPServiceRecord!)
```

## Parameters 

`inSDPServiceRecord`  

## See Also

### Initializers

init!(device: IOBluetoothDevice!, channelID: BluetoothRFCOMMChannelID)

Initializes a Bluetooth-based OBEX Session using a Bluetooth device.

init!(incomingRFCOMMChannel: IOBluetoothRFCOMMChannel!, eventSelector: Selector!, selectorTarget: Any!, refCon: UnsafeMutableRawPointer!)

Initializes a Bluetooth-based OBEX Session using an incoming RFCOMM channel.

