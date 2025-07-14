

- MailKit
- MEOutgoingMessageEncodingStatus
-  canEncrypt 

Instance Property

# canEncrypt

A Boolean value that indicates the message security handler can encrypt the outgoing message.

macOS 12.0+

``` source
var canEncrypt: Bool { get }
```

## See Also

### Providing Encoding Status

init(canSign: Bool, canEncrypt: Bool, securityError: (any Error)?, addressesFailingEncryption: [MEEmailAddress])

Creates an object that describes whether the message security handler can encrypt or sign an outgoing message.

var canSign: Bool

A Boolean value that indicates the message security handler can digitally sign the outgoing message.

var securityError: (any Error)?

An error that the message encoder encountered while determining the encoding status for the outgoing message.

var addressesFailingEncryption: [MEEmailAddress]

An array of email addresses that prevent the message security handler from signing the message.

