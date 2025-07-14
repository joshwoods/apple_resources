

- Core NFC
-  NFCNDEFMessage 

Class

# NFCNDEFMessage

An NFC NDEF message consisting of an array of payload records.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class NFCNDEFMessage
```

## Topics

### Creating an NDEF Message

init(records: [NFCNDEFPayload])

Creates an NDEF message with the specified records.

convenience init?(data: Data)

Creates an NDEF message from raw data representing the message.

### Accessing NDEF Records

var records: [NFCNDEFPayload]

An array of records for the message.

### Getting the Message Length

var length: Int

The length, in bytes, of the NDEF message when stored on an NFC tag.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### NDEF messages and payloads

class NFCNDEFPayload

A payload record in an NFC NDEF message.

