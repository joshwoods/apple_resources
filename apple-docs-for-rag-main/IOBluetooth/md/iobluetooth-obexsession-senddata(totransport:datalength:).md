

- IOBluetooth
- OBEXSession
-  sendData(toTransport:dataLength:) 

Instance Method

# sendData(toTransport:dataLength:)

You must override this to send data over your transport. This does nothing by default, it will return a kOBEXUnsupportedError.

macOS

``` source
func sendData(
    toTransport inDataToSend: UnsafeMutableRawPointer!,
    dataLength inDataLength: Int
) -> OBEXError
```

## Parameters 

`inDataToSend`  

Data to shove over the transport to a remote OBEX session.

`inDataLength`  

Length of data passed in.

## Discussion

Tranport subclasses must override this! When called you should send the data over the transport to the remote session.

