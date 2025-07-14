

- MailKit
- MEMessage
-  allRecipientAddresses 

Instance Property

# allRecipientAddresses

An array of email addresses for all recipients of the message.

macOS 12.0+

``` source
var allRecipientAddresses: [MEEmailAddress] { get }
```

## Discussion

This property contains all values in toAddresses, ccAddresses, and bccAddresses.

The entries in the array specify the email addresses only, and don’t include any additional text. For example, if the recipient headers in the message includes `Maria Ruiz `, the array contains `mruiz2@icloud.com`.

## See Also

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

