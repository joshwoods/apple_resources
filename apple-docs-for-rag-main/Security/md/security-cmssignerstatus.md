

- Security
-  CMSSignerStatus 

Enumeration

# CMSSignerStatus

The constants that indicate the status of the signature and signer information in a signed message.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum CMSSignerStatus
```

## Overview

These are obtained using the CMSDecoderCopySignerStatus(_:_:_:_:_:_:_:) function.

## Topics

### Constants

case unsigned

The message was not signed.

case valid

The message was signed and both the signature and the signer certificate have been verified.

case needsDetachedContent

The message was signed but has detached content. You must call the CMSDecoderSetDetachedContent(_:_:) function before ascertaining the signature status.

case invalidSignature

The message was signed but the signature is invalid.

case invalidCert

The message was signed but the signer’s certificate could not be verified.

case invalidIndex

The specified value for the signer index (`signerIndex` parameter) is greater than the number of signers of the message minus one (`signerIndex > (numSigners – 1)`).

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

