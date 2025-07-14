

- MailKit
-  MEMessageEncodingResult 

Class

# MEMessageEncodingResult

An object that contains a signed or encrypted message, or errors that indicate failure to encode the message.

macOS 12.0+

``` source
class MEMessageEncodingResult
```

## Topics

### Providing an Encoding Result

init(encodedMessage: MEEncodedOutgoingMessage?, signingError: (any Error)?, encryptionError: (any Error)?)

Creates an encoding result object with a signed or encrypted message, or errors if the message encoder fails to encode the message.

var encodedMessage: MEEncodedOutgoingMessage?

A signed or encrypted message, if the message security handler needs to encode the message.

var encryptionError: (any Error)?

An error that occurred while the message encoder encrypted the message.

var signingError: (any Error)?

An error that occurred while the message encoder signed the message.

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

class MEEncodedOutgoingMessage

An object that contains the signed or encrypted representation of a message’s RFC 2822 data.

class MEOutgoingMessageEncodingStatus

An object that contains information about security measures the user can apply when composing a message.

