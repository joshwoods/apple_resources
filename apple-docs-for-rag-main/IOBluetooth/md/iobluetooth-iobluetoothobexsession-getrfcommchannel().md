

- IOBluetooth
- IOBluetoothOBEXSession
-  getRFCOMMChannel() 

Instance Method

# getRFCOMMChannel()

Get the Bluetooth RFCOMM channel being used by the session object.

macOS

``` source
func getRFCOMMChannel() -> IOBluetoothRFCOMMChannel!
```

## Return Value

A IOBluetoothRFCOMMChannel object.

## Discussion

This could potentially be nil even though you have a valid OBEX session, because the RFCOMM channel is only valid when the session is connected.

