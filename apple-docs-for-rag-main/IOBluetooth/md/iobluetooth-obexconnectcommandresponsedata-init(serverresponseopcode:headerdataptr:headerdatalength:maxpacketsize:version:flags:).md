

- IOBluetooth
- OBEXConnectCommandResponseData
-  init(serverResponseOpCode:headerDataPtr:headerDataLength:maxPacketSize:version:flags:) 

Initializer

# init(serverResponseOpCode:headerDataPtr:headerDataLength:maxPacketSize:version:flags:)

macOS

``` source
init(
    serverResponseOpCode: OBEXOpCode,
    headerDataPtr: UnsafeMutableRawPointer!,
    headerDataLength: Int,
    maxPacketSize: OBEXMaxPacketLength,
    version: OBEXVersion,
    flags: OBEXFlags
)
```

