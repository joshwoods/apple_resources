

- MailKit
-  MEMessageDecoder 

Protocol

# MEMessageDecoder

An object that decrypts messages and provides details about digital signatures.

macOS 12.0+

``` source
protocol MEMessageDecoder : NSObjectProtocol
```

## Topics

### Decrypting Messages and Verifying Signatures

func decodedMessage(forMessageData: Data) -> MEDecodedMessage?

Decrypts message content and details about digital signatures.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- MEMessageSecurityHandler

## See Also

### Decrypting Messages and Verifying Signatures

class MEDecodedMessage

An object that contains the RFC 2822 data for a message, without encryption or digital signatures.

class MEMessageSigner

An object that contains details about the person who signed a message.

class MEMessageSecurityInformation

An object that contains details about a message’s content, such as if it’s encrypted and who digitally signed it.

