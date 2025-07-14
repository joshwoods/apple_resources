

- MailKit
-  MEEncodedOutgoingMessage 

Class

# MEEncodedOutgoingMessage

An object that contains the signed or encrypted representation of a message’s RFC 2822 data.

macOS 12.0+

``` source
class MEEncodedOutgoingMessage
```

## Overview

When MailKit invokes your message security handler’s encode(_:composeContext:completionHandler:) method, it digitally signs and encrypts the message. After encoding the message data, create an instance of MEEncodedOutgoingMessage to pass back to MailKit. Set the isSigned and isEncrypted values to indicate how you encoded the message.

## Topics

### Encoding Outgoing Messages

init(rawData: Data, isSigned: Bool, isEncrypted: Bool)

Creates an object that contains the outgoing message’s encoded data, and indicates if the encoder encrypted or signed the message.

var isEncrypted: Bool

A Boolean value that indicates if the message encoder encrypted the message.

var isSigned: Bool

A Boolean value that indicates if the message encoder signed the message.

var rawData: Data

The encrypted, signed, or both encrypted and signed data for the outgoing message.

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

### Encrypting and Signing Messages

protocol MEMessageEncoder

An object that encrypts or digitally signs outgoing messages.

class MEOutgoingMessageEncodingStatus

An object that contains information about security measures the user can apply when composing a message.

class MEMessageEncodingResult

An object that contains a signed or encrypted message, or errors that indicate failure to encode the message.

