

- Core NFC
- NFCISO7816APDU
-  init(instructionClass:instructionCode:p1Parameter:p2Parameter:data:expectedResponseLength:) 

Initializer

# init(instructionClass:instructionCode:p1Parameter:p2Parameter:data:expectedResponseLength:)

Creates an APDU object with the instruction class and code, parameter bytes, and expected response length.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
init(
    instructionClass: UInt8,
    instructionCode: UInt8,
    p1Parameter: UInt8,
    p2Parameter: UInt8,
    data: Data,
    expectedResponseLength: Int
)
```

## Parameters 

`instructionClass`  

The instruction class (CLA) byte value.

`instructionCode`  

The instruction code (INS) byte value.

`p1Parameter`  

The P1 parameter byte value.

`p2Parameter`  

The P2 parameter byte value.

`data`  

The data to transmit. The APDU object specifies the length of the transmission data in the Lc field.

`expectedResponseLength`  

The expected response data length (Le) in bytes. The value should be one of the following:

- A length between 1 and 65536 inclusively.

- –1 when you expect no response data.

- 256 to send `00` as the short Le field value, assuming the data field is less than 256 bytes.

- 65536 to send `0000` as the extended Le field.

## Return Value

A newly initialized ISO 7816 APDU object.

## Discussion

If your app needs more precise control of the APDU format, use init(data:) to create the APDU object.

## See Also

### Creating an APDU Object

init?(data: Data)

Creates an APDU object with the data buffer containing the full APDU.

