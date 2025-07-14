

- MailKit
- MEMessageSecurityInformation
-  encryptionError 

Instance Property

# encryptionError

An error that indicates the security handler couldn’t decrypt the message.

macOS 12.0+

``` source
var encryptionError: (any Error)? { get }
```

## See Also

### Describing Message Security Attributes

init(signers: [MEMessageSigner], isEncrypted: Bool, signingError: (any Error)?, encryptionError: (any Error)?)

Creates a message security information object that indicates if a message is encrypted, who signed it, or if an error occurred when decoding the message.

var isEncrypted: Bool

A Boolean value that indicates if the sender encrypted the message.

var signers: [MEMessageSigner]

An array of objects that contain information about who signed the message.

var signingError: (any Error)?

An error that indicates the security handler couldn’t decode the message’s digital signatures.

