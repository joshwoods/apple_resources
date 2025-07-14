

- IOBluetooth
- OBEXConnectCommandData
-  init(headerDataPtr:headerDataLength:maxPacketSize:version:flags:) 

Initializer

# init(headerDataPtr:headerDataLength:maxPacketSize:version:flags:)

macOS

``` source
init(
    headerDataPtr: UnsafeMutableRawPointer!,
    headerDataLength: Int,
    maxPacketSize: OBEXMaxPacketLength,
    version: OBEXVersion,
    flags: OBEXFlags
)
```

