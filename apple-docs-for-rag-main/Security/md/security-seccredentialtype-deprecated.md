

- Security
-  SecCredentialType Deprecated

Enumeration

# SecCredentialType

The credential type to be returned by SecKeyGetCredentials.

macOS 10.3–12.0Deprecated

``` source
enum SecCredentialType
```

Deprecated

No longer supported

## Overview

See the section “Servers and the Keychain” in the macOS Keychain Services Tasks chapter of Keychain Services Programming Guide for information on the use of UI with keychain tasks.

## Topics

### Constants

case `default`

The default setting for determining whether to present UI is used.

case withUI

Keychain operations on keys that have this credential are allowed to present UI if required.

case noUI

Keychain operations on keys that have this credential are not allowed to present UI, and will fail if UI is required.

### Initializers

init?(rawValue: uint32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

