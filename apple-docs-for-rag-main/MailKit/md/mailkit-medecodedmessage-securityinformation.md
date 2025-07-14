

- MailKit
- MEDecodedMessage
-  securityInformation 

Instance Property

# securityInformation

An object that contains encryption and digital signature information about the message content.

macOS 12.0+

``` source
var securityInformation: MEMessageSecurityInformation { get }
```

## See Also

### Decoding Messages

var rawData: Data?

The decoded MIME data for a message.

