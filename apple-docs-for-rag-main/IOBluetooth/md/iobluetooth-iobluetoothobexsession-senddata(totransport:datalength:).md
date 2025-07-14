

- IOBluetooth
- IOBluetoothOBEXSession
-  sendData(toTransport:dataLength:) 

Instance Method

# sendData(toTransport:dataLength:)

An OBEXSession override. When this is called by the session baseclass, we will send the data we are given over our transport connection. If none is open, we could try to open it, or just return an error. In our case, it will be sent over the RFCOMM channel.

macOS

``` source
func sendData(
    toTransport inDataToSend: UnsafeMutableRawPointer!,
    dataLength inDataLength: Int
) -> OBEXError
```

