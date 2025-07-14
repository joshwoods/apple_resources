

- Core NFC
-  NFCVASResponse 

Class

# NFCVASResponse

An object representing the response from a single `GET VAS DATA` command.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class NFCVASResponse
```

## Topics

### Getting the Response Status

var status: NFCVASResponse.ErrorCode

A response APDU status code.

typealias VASErrorCode

Constants representing APDU status codes for a VAS response.

Deprecated

### Getting the VAS Data

var vasData: Data

A data object containing the VAS data.

### Getting the Mobile Token

var mobileToken: Data

A mobile token value.

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

### Receiving VAS Responses

func readerSession(NFCVASReaderSession, didReceive: [NFCVASResponse])

Tells the delegate that the reader session received a VAS response.

**Required**

