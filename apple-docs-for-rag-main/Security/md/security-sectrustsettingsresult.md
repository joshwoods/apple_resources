

- Security
-  SecTrustSettingsResult 

Enumeration

# SecTrustSettingsResult

Trust settings returned in usage constraints dictionaries.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum SecTrustSettingsResult
```

## Overview

These values appear in the usage constraints dictionaries returned by the SecTrustSettingsCopyTrustSettings(_:_:_:) and SecTrustSettingsSetTrustSettings(_:_:_:) functions.

## Topics

### Constants

case invalid

Never valid in a trust settings array or in an API call.

case trustRoot

This root certificate is explicitly trusted.

case trustAsRoot

This non-root certificate is explicitly trusted as if it were a trusted root.

case deny

This certificate is explicitly distrusted.

case unspecified

This certificate is neither trusted nor distrusted. This value can be used to specify an “allowed error” without assigning trust to a specific certificate.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

