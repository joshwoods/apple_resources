

- MailKit
- MEMessageEncodingResult
-  encryptionError 

Instance Property

# encryptionError

An error that occurred while the message encoder encrypted the message.

macOS 12.0+

``` source
var encryptionError: (any Error)? { get }
```

## See Also

### Providing an Encoding Result

init(encodedMessage: MEEncodedOutgoingMessage?, signingError: (any Error)?, encryptionError: (any Error)?)

Creates an encoding result object with a signed or encrypted message, or errors if the message encoder fails to encode the message.

var encodedMessage: MEEncodedOutgoingMessage?

A signed or encrypted message, if the message security handler needs to encode the message.

var signingError: (any Error)?

An error that occurred while the message encoder signed the message.

