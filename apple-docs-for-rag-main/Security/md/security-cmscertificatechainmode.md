

- Security
-  CMSCertificateChainMode 

Enumeration

# CMSCertificateChainMode

Constants that can be set to specify what certificates to include in a signed message.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum CMSCertificateChainMode
```

## Overview

Use these with the CMSEncoderSetCertificateChainMode(_:_:) function.

## Topics

### Constants

case none

Don’t include any certificates.

case signerOnly

Only include signer certificates.

case chain

Include the signer certificate chain up to but not including the root certificate.

case chainWithRoot

Include the entire signer certificate chain, including the root certificate.

### Enumeration Cases

case chainWithRootOrFail

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

