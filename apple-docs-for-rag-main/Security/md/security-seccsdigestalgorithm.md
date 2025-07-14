

- Security
-  SecCSDigestAlgorithm 

Enumeration

# SecCSDigestAlgorithm

The list of digest algorithms available for code signatures.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum SecCSDigestAlgorithm
```

## Overview

Use these values with the kSecCodeInfoDigestAlgorithm and kSecCodeInfoDigestAlgorithms keys described in Signing Information Dictionary Keys.

## Topics

### Enumeration Cases

case codeSignatureHashSHA1

case codeSignatureHashSHA256

case codeSignatureHashSHA256Truncated

case codeSignatureHashSHA384

case codeSignatureHashSHA512

case codeSignatureNoHash

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

