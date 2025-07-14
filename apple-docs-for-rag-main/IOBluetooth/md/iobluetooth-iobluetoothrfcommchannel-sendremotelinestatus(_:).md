

- IOBluetooth
- IOBluetoothRFCOMMChannel
-  sendRemoteLineStatus(\_:) 

Instance Method

# sendRemoteLineStatus(\_:)

Sends an error to the remote side.

macOS

``` source
func sendRemoteLineStatus(_ lineStatus: BluetoothRFCOMMLineStatus) -> IOReturn
```

## Parameters 

`lineStatus`  

The error type. The error code can be NoError, OverrunError, ParityError or FramingError.

## Return Value

An error code value. 0 if successful.

