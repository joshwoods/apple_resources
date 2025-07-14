

- MailKit
- MEMessageSecurityInformation
-  signingError 

Instance Property

# signingError

An error that indicates the security handler couldn’t decode the message’s digital signatures.

macOS 12.0+

``` source
var signingError: (any Error)? { get }
```

## See Also

### Describing Message Security Attributes

init(signers: [MEMessageSigner], isEncrypted: Bool, signingError: (any Error)?, encryptionError: (any Error)?)

Creates a message security information object that indicates if a message is encrypted, who signed it, or if an error occurred when decoding the message.

var isEncrypted: Bool

A Boolean value that indicates if the sender encrypted the message.

var encryptionError: (any Error)?

An error that indicates the security handler couldn’t decrypt the message.

var signers: [MEMessageSigner]

An array of objects that contain information about who signed the message.

