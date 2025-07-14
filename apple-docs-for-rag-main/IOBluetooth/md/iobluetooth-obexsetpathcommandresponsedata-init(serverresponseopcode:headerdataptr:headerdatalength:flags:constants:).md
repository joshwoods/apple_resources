

- IOBluetooth
- OBEXSetPathCommandResponseData
-  init(serverResponseOpCode:headerDataPtr:headerDataLength:flags:constants:) 

Initializer

# init(serverResponseOpCode:headerDataPtr:headerDataLength:flags:constants:)

macOS

``` source
init(
    serverResponseOpCode: OBEXOpCode,
    headerDataPtr: UnsafeMutableRawPointer!,
    headerDataLength: Int,
    flags: OBEXFlags,
    constants: OBEXConstants
)
```

