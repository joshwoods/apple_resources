

- IOBluetooth
- IOBluetoothOBEXSession
-  closeTransportConnection() 

Instance Method

# closeTransportConnection()

An OBEXSession override. When this is called by the session baseclass, we will close the transport connection if it is opened. In our case, it will be the RFCOMM channel that needs closing.

macOS

``` source
func closeTransportConnection() -> OBEXError
```

## Return Value

Success or failure code, describing whether the call succeeded in closing the transport connection successfully.

