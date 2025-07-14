

- Core NFC
- NFCISO7816APDU
-  init(data:) 

Initializer

# init(data:)

Creates an APDU object with the data buffer containing the full APDU.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
init?(data: Data)
```

## Parameters 

`data`  

A data buffer containing the full APDU.

## Return Value

A newly initialized APDU object.

## See Also

### Creating an APDU Object

init(instructionClass: UInt8, instructionCode: UInt8, p1Parameter: UInt8, p2Parameter: UInt8, data: Data, expectedResponseLength: Int)

Creates an APDU object with the instruction class and code, parameter bytes, and expected response length.

