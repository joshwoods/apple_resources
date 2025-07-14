

- MailKit
- MEEncodedOutgoingMessage
-  isEncrypted 

Instance Property

# isEncrypted

A Boolean value that indicates if the message encoder encrypted the message.

macOS 12.0+

``` source
var isEncrypted: Bool { get }
```

## See Also

### Encoding Outgoing Messages

init(rawData: Data, isSigned: Bool, isEncrypted: Bool)

Creates an object that contains the outgoing message’s encoded data, and indicates if the encoder encrypted or signed the message.

var isSigned: Bool

A Boolean value that indicates if the message encoder signed the message.

var rawData: Data

The encrypted, signed, or both encrypted and signed data for the outgoing message.

