

- IOBluetooth
- OBEXSession
-  serverHandleIncomingData(\_:) 

Instance Method

# serverHandleIncomingData(\_:)

Tranport subclasses need to invoke this from their own data-receive handlers. For example, when data is received over a Bluetooth RFCOMM channel in the IOBluetoothOBEXSession, it in turn calls this to dispatch the data. If you do not handle this case, your server session will not work, guaranteed.

macOS

``` source
func serverHandleIncomingData(_ event: UnsafeMutablePointer!)
```

## Parameters 

`event`  

New event received from the transport.

## Discussion

Tranport subclasses must call this for OBEX server sessions to work!

