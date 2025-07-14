

- MailKit
- MEEncodedOutgoingMessage
-  init(rawData:isSigned:isEncrypted:) 

Initializer

# init(rawData:isSigned:isEncrypted:)

Creates an object that contains the outgoing message’s encoded data, and indicates if the encoder encrypted or signed the message.

macOS 12.0+

``` source
init(
    rawData: Data,
    isSigned: Bool,
    isEncrypted: Bool
)
```

## Parameters 

`rawData`  

The encrypted, signed, or both encrypted and signed message data.

`isSigned`  

A Boolean value that indicates if the data contains a signed message.

`isEncrypted`  

A Boolean value that indicates if the data contains an encrypted message.

## See Also

### Encoding Outgoing Messages

var isEncrypted: Bool

A Boolean value that indicates if the message encoder encrypted the message.

var isSigned: Bool

A Boolean value that indicates if the message encoder signed the message.

var rawData: Data

The encrypted, signed, or both encrypted and signed data for the outgoing message.

