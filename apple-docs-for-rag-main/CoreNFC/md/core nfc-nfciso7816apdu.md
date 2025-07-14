

- Core NFC
-  NFCISO7816APDU 

Class

# NFCISO7816APDU

An object representing an ISO 7816 application protocol data unit (APDU).

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class NFCISO7816APDU
```

## Topics

### Creating an APDU Object

init(instructionClass: UInt8, instructionCode: UInt8, p1Parameter: UInt8, p2Parameter: UInt8, data: Data, expectedResponseLength: Int)

Creates an APDU object with the instruction class and code, parameter bytes, and expected response length.

init?(data: Data)

Creates an APDU object with the data buffer containing the full APDU.

### Getting the Instruction Bytes

var instructionClass: UInt8

The value of the instruction class (CLA) byte.

var instructionCode: UInt8

The value of the instruction code (INS) byte.

### Get the Parameter Bytes

var p1Parameter: UInt8

The value of the P1 parameter byte.

var p2Parameter: UInt8

The value of the P2 parameter byte.

### Getting the APDU Data

var data: Data?

The data to transmit.

### Getting the Expected Response Length

var expectedResponseLength: Int

The expected response data length (Le) in bytes.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Sending a Command

func sendCommand(apdu: NFCISO7816APDU, resultHandler: (Result&lt;NFCISO7816ResponseAPDU, any Error>) -> Void)

Sends an application protocol data unit (APDU) to the tag and receives a response APDU.

func sendCommand(apdu: NFCISO7816APDU, completionHandler: (Data, UInt8, UInt8, (any Error)?) -> Void)

Sends an application protocol data unit (APDU) to the tag and receives a response APDU.

**Required** Default implementation provided.

struct NFCISO7816ResponseAPDU

An object containing the response from the tag.

