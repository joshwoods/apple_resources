

- MailKit
-  MEOutgoingMessageEncodingStatus 

Class

# MEOutgoingMessageEncodingStatus

An object that contains information about security measures the user can apply when composing a message.

macOS 12.0+

``` source
class MEOutgoingMessageEncodingStatus
```

## Overview

As a user composes a new message, MailKit requests the encoding status from your message security handler. The handler provides an MEOutgoingMessageEncodingStatus that contains:

- Boolean values that indicate if the handler can sign or encrypt the message

- An error if verifying the security status fails

- An array of recipient addresses for which the handler can’t encrypt the message

## Topics

### Providing Encoding Status

init(canSign: Bool, canEncrypt: Bool, securityError: (any Error)?, addressesFailingEncryption: [MEEmailAddress])

Creates an object that describes whether the message security handler can encrypt or sign an outgoing message.

var canSign: Bool

A Boolean value that indicates the message security handler can digitally sign the outgoing message.

var canEncrypt: Bool

A Boolean value that indicates the message security handler can encrypt the outgoing message.

var securityError: (any Error)?

An error that the message encoder encountered while determining the encoding status for the outgoing message.

var addressesFailingEncryption: [MEEmailAddress]

An array of email addresses that prevent the message security handler from signing the message.

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

### Encrypting and Signing Messages

protocol MEMessageEncoder

An object that encrypts or digitally signs outgoing messages.

class MEEncodedOutgoingMessage

An object that contains the signed or encrypted representation of a message’s RFC 2822 data.

class MEMessageEncodingResult

An object that contains a signed or encrypted message, or errors that indicate failure to encode the message.

