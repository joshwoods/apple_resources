

- MailKit
- MEOutgoingMessageEncodingStatus
-  init(canSign:canEncrypt:securityError:addressesFailingEncryption:) 

Initializer

# init(canSign:canEncrypt:securityError:addressesFailingEncryption:)

Creates an object that describes whether the message security handler can encrypt or sign an outgoing message.

macOS 12.0+

``` source
init(
    canSign: Bool,
    canEncrypt: Bool,
    securityError: (any Error)?,
    addressesFailingEncryption: [MEEmailAddress]
)
```

## Parameters 

`canSign`  

A Boolean value that indicates the message security handler can digitally sign the outgoing message.

`canEncrypt`  

A Boolean value that indicates the message security handler can encrypt the outgoing message.

`securityError`  

An error that indicates a failure while determining the encoding status for the outgoing message.

`addressesFailingEncryption`  

An array of email addresses that prevent the message security handler from signing the message.

## See Also

### Providing Encoding Status

var canSign: Bool

A Boolean value that indicates the message security handler can digitally sign the outgoing message.

var canEncrypt: Bool

A Boolean value that indicates the message security handler can encrypt the outgoing message.

var securityError: (any Error)?

An error that the message encoder encountered while determining the encoding status for the outgoing message.

var addressesFailingEncryption: [MEEmailAddress]

An array of email addresses that prevent the message security handler from signing the message.

