

- MailKit
- MEMessageSigner
-  init(emailAddresses:signatureLabel:context:) 

Initializer

# init(emailAddresses:signatureLabel:context:)

Creates a new message signer object that contains the email addresses of the signers, a label, and context data.

macOS 12.0+

``` source
init(
    emailAddresses: [MEEmailAddress],
    signatureLabel label: String,
    context: Data?
)
```

## Parameters 

`emailAddresses`  

An array of email addresses associated with the signature.

`label`  

The message signer’s label that Mail shows in the message’s headers.

`context`  

Data related to the message signature, such as the signing certificate.

## See Also

### Describing Message Signers

var emailAddresses: [MEEmailAddress]

An array of email addresses associated with the signature.

var label: String

A string that the message’s headers use to display the message signer.

var context: Data

Data related to the message signature, such as the signing certificate.

