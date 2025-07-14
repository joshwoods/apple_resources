

- MailKit
- MEMessageEncodingResult
-  init(encodedMessage:signingError:encryptionError:) 

Initializer

# init(encodedMessage:signingError:encryptionError:)

Creates an encoding result object with a signed or encrypted message, or errors if the message encoder fails to encode the message.

macOS 12.0+

``` source
init(
    encodedMessage: MEEncodedOutgoingMessage?,
    signingError: (any Error)?,
    encryptionError: (any Error)?
)
```

## Parameters 

`encodedMessage`  

A signed or encrypted message.

`signingError`  

An error that occurred while signing the message.

`encryptionError`  

An error that occurred while encrypting the message.

## Discussion

If the message doesn’t require a digital signature or any encryption, specify `nil` for the message and errors.

If the message security handler does need to sign or encrypt the message, but encoding fails, specify `nil` for `encodedMessage`, and an error for one or both of the error parameters.

## See Also

### Providing an Encoding Result

var encodedMessage: MEEncodedOutgoingMessage?

A signed or encrypted message, if the message security handler needs to encode the message.

var encryptionError: (any Error)?

An error that occurred while the message encoder encrypted the message.

var signingError: (any Error)?

An error that occurred while the message encoder signed the message.

