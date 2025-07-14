

- IOBluetooth
- IOBluetoothOBEXSession
-  hasOpenTransportConnection() 

Instance Method

# hasOpenTransportConnection()

An OBEXSession override. When this is called by the session baseclass, we will return whether or not we have a transport connection established to another OBEX server/client. In our case we will tell whether or not the RFCOMM channel to a remote device is still open.

macOS

``` source
func hasOpenTransportConnection() -> Bool
```

## Return Value

True or false, whether there is already an open transport connection for this OBEX session.

