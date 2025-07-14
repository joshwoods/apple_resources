

- MailKit
-  MEMessage 

Class

# MEMessage

An object that contains information about a mail message, such as the subject, addressees, date sent, and the message contents.

macOS 12.0+

``` source
class MEMessage
```

## Topics

### Accessing the Sender and Recipients

var fromAddress: MEEmailAddress

The sender’s email address.

var toAddresses: [MEEmailAddress]

An array of email addresses for the primary recipients of the message.

var ccAddresses: [MEEmailAddress]

An array of email addresses for the secondary recipients of the message.

var bccAddresses: [MEEmailAddress]

An array of email addresses for the concealed tertiary recipients of the message.

var replyToAddresses: [MEEmailAddress]

An array of email addresses to use when replying to the message.

var allRecipientAddresses: [MEEmailAddress]

An array of email addresses for all recipients of the message.

### Accessing the Message Subject

var subject: String

The subject of the message.

### Accessing Message Content

var headers: [String : [String]]?

A dictionary that contains the message’s header values.

var rawData: Data?

The raw RFC 2822 header and body content of the message.

### Accessing Message State

var state: MEMessageState

The state of the mail message.

### Instance Properties

var encryptionState: MEMessageEncryptionState

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

### Message Properties

enum MEMessageState

The state of a message: sent, unsent, or received.

