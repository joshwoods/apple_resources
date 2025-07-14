

- MailKit
- MEEncodedOutgoingMessage
-  isSigned 

Instance Property

# isSigned

A Boolean value that indicates if the message encoder signed the message.

macOS 12.0+

``` source
var isSigned: Bool { get }
```

## See Also

### Encoding Outgoing Messages

init(rawData: Data, isSigned: Bool, isEncrypted: Bool)

Creates an object that contains the outgoing message’s encoded data, and indicates if the encoder encrypted or signed the message.

var isEncrypted: Bool

A Boolean value that indicates if the message encoder encrypted the message.

var rawData: Data

The encrypted, signed, or both encrypted and signed data for the outgoing message.

