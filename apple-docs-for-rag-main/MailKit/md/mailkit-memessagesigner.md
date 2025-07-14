

- MailKit
-  MEMessageSigner 

Class

# MEMessageSigner

An object that contains details about the person who signed a message.

macOS 12.0+

``` source
class MEMessageSigner
```

## Topics

### Describing Message Signers

init(emailAddresses: [MEEmailAddress], signatureLabel: String, context: Data?)

Creates a new message signer object that contains the email addresses of the signers, a label, and context data.

var emailAddresses: [MEEmailAddress]

An array of email addresses associated with the signature.

var label: String

A string that the message’s headers use to display the message signer.

var context: Data

Data related to the message signature, such as the signing certificate.

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

class MEMessageSecurityInformation

An object that contains details about a message’s content, such as if it’s encrypted and who digitally signed it.

