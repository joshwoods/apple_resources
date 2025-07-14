

- MailKit
-  MEDecodedMessage 

Class

# MEDecodedMessage

An object that contains the RFC 2822 data for a message, without encryption or digital signatures.

macOS 12.0+

``` source
class MEDecodedMessage
```

## Overview

When MailKit invokes your message security handler’s decodedMessage(forMessageData:) method, you decode the message data and return an instance of MEDecodedMessage that contains unencrypted MIME data.

## Topics

### Decoding Messages

var rawData: Data?

The decoded MIME data for a message.

var securityInformation: MEMessageSecurityInformation

An object that contains encryption and digital signature information about the message content.

### Initializers

init(data: Data?, securityInformation: MEMessageSecurityInformation, context: Data?)

init(data: Data?, securityInformation: MEMessageSecurityInformation, context: Data?, banner: MEDecodedMessageBanner?)

### Instance Properties

var banner: MEDecodedMessageBanner?

var context: Data?

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

class MEMessageSigner

An object that contains details about the person who signed a message.

class MEMessageSecurityInformation

An object that contains details about a message’s content, such as if it’s encrypted and who digitally signed it.

