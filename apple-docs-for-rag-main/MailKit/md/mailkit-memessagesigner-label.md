

- MailKit
- MEMessageSigner
-  label 

Instance Property

# label

A string that the message’s headers use to display the message signer.

macOS 12.0+

``` source
var label: String { get }
```

## See Also

### Describing Message Signers

init(emailAddresses: [MEEmailAddress], signatureLabel: String, context: Data?)

Creates a new message signer object that contains the email addresses of the signers, a label, and context data.

var emailAddresses: [MEEmailAddress]

An array of email addresses associated with the signature.

var context: Data

Data related to the message signature, such as the signing certificate.

