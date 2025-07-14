

- MailKit
- MEMessage
-  fromAddress 

Instance Property

# fromAddress

The sender’s email address.

macOS 12.0+

``` source
@NSCopying
var fromAddress: MEEmailAddress { get }
```

## Discussion

This property corresponds to the From header in the message.

The value specifies the email address only, and doesn’t include any additional text. For example, if the From header in the message is `Maria Ruiz `, the value of this property is `mruiz2@icloud.com`.

## See Also

### Accessing the Sender and Recipients

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

