

- MailKit
-  MEMessageEncoder 

Protocol

# MEMessageEncoder

An object that encrypts or digitally signs outgoing messages.

macOS 12.0+

``` source
protocol MEMessageEncoder : NSObjectProtocol
```

## Topics

### Instance Methods

func encode(MEMessage, composeContext: MEComposeContext, completionHandler: (MEMessageEncodingResult) -> Void)

**Required**

func getEncodingStatus(for: MEMessage, composeContext: MEComposeContext, completionHandler: (MEOutgoingMessageEncodingStatus) -> Void)

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- MEMessageSecurityHandler

## See Also

### Encrypting and Signing Messages

class MEEncodedOutgoingMessage

An object that contains the signed or encrypted representation of a message’s RFC 2822 data.

class MEOutgoingMessageEncodingStatus

An object that contains information about security measures the user can apply when composing a message.

class MEMessageEncodingResult

An object that contains a signed or encrypted message, or errors that indicate failure to encode the message.

