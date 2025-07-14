

- IOBluetooth
- IOBluetoothOBEXSession
-  init(incomingRFCOMMChannel:eventSelector:selectorTarget:refCon:) 

Initializer

# init(incomingRFCOMMChannel:eventSelector:selectorTarget:refCon:)

Initializes a Bluetooth-based OBEX Session using an incoming RFCOMM channel.

macOS

``` source
init!(
    incomingRFCOMMChannel inChannel: IOBluetoothRFCOMMChannel!,
    eventSelector inEventSelector: Selector!,
    selectorTarget inEventSelectorTarget: Any!,
    refCon inUserRefCon: UnsafeMutableRawPointer!
)
```

## Parameters 

`inChannel`  

RFCOMM channel ID of the desired channel to be used.

`inEventSelector`  

The selector to be called when an event is received.

`inEventSelectorTarget`  

The target object that get the selector message.

`inUserRefCon`  

Caller reference constant, pass whatever you want, it will be returned to you in the selector.

## See Also

### Initializers

init!(device: IOBluetoothDevice!, channelID: BluetoothRFCOMMChannelID)

Initializes a Bluetooth-based OBEX Session using a Bluetooth device.

init!(sdpServiceRecord: IOBluetoothSDPServiceRecord!)

Initializes a Bluetooth-based OBEX Session using an SDP service record.

