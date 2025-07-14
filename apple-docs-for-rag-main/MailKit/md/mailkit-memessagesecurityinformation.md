

- MailKit
-  MEMessageSecurityInformation 

Class

# MEMessageSecurityInformation

An object that contains details about a message’s content, such as if it’s encrypted and who digitally signed it.

macOS 12.0+

``` source
class MEMessageSecurityInformation
```

## Topics

### Describing Message Security Attributes

init(signers: [MEMessageSigner], isEncrypted: Bool, signingError: (any Error)?, encryptionError: (any Error)?)

Creates a message security information object that indicates if a message is encrypted, who signed it, or if an error occurred when decoding the message.

var isEncrypted: Bool

A Boolean value that indicates if the sender encrypted the message.

var encryptionError: (any Error)?

An error that indicates the security handler couldn’t decrypt the message.

var signers: [MEMessageSigner]

An array of objects that contain information about who signed the message.

var signingError: (any Error)?

An error that indicates the security handler couldn’t decode the message’s digital signatures.

### Initializers

init(signers: [MEMessageSigner], isEncrypted: Bool, signingError: (any Error)?, encryptionError: (any Error)?, shouldBlockRemoteContent: Bool, localizedRemoteContentBlockingReason: String?)

### Instance Properties

var localizedRemoteContentBlockingReason: String?

var shouldBlockRemoteContent: Bool

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

### Decrypting Messages and Verifying Signatures

protocol MEMessageDecoder

An object that decrypts messages and provides details about digital signatures.

class MEDecodedMessage

An object that contains the RFC 2822 data for a message, without encryption or digital signatures.

class MEMessageSigner

An object that contains details about the person who signed a message.

