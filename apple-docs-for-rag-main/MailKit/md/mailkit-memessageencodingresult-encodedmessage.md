

- MailKit
- MEMessageEncodingResult
-  encodedMessage 

Instance Property

# encodedMessage

A signed or encrypted message, if the message security handler needs to encode the message.

macOS 12.0+

``` source
@NSCopying
var encodedMessage: MEEncodedOutgoingMessage? { get }
```

## Discussion

If the message security handler doesn’t need to apply security measures to the outgoing message, the value of this property is `nil`.

## See Also

### Providing an Encoding Result

init(encodedMessage: MEEncodedOutgoingMessage?, signingError: (any Error)?, encryptionError: (any Error)?)

Creates an encoding result object with a signed or encrypted message, or errors if the message encoder fails to encode the message.

var encryptionError: (any Error)?

An error that occurred while the message encoder encrypted the message.

var signingError: (any Error)?

An error that occurred while the message encoder signed the message.

