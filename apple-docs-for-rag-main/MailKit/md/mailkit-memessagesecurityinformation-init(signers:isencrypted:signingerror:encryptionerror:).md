

- MailKit
- MEMessageSecurityInformation
-  init(signers:isEncrypted:signingError:encryptionError:) 

Initializer

# init(signers:isEncrypted:signingError:encryptionError:)

Creates a message security information object that indicates if a message is encrypted, who signed it, or if an error occurred when decoding the message.

macOS 12.0+

``` source
init(
    signers: [MEMessageSigner],
    isEncrypted: Bool,
    signingError: (any Error)?,
    encryptionError: (any Error)?
)
```

## Parameters 

`signers`  

An array of objects that contain information about who signed the message.

`isEncrypted`  

A Boolean value that indicates if the message is encrypted.

`signingError`  

An error that indicates the security handler couldn’t decode the message’s digital signatures.

`encryptionError`  

An error that indicates the security handler couldn’t decrypt the message.

## See Also

### Describing Message Security Attributes

var isEncrypted: Bool

A Boolean value that indicates if the sender encrypted the message.

var encryptionError: (any Error)?

An error that indicates the security handler couldn’t decrypt the message.

var signers: [MEMessageSigner]

An array of objects that contain information about who signed the message.

var signingError: (any Error)?

An error that indicates the security handler couldn’t decode the message’s digital signatures.

