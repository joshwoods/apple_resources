

- Security
-  SecTrustSettingsDomain 

Enumeration

# SecTrustSettingsDomain

The trust settings domains.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum SecTrustSettingsDomain
```

## Topics

### Constants

case user

Per-user trust settings.

case admin

Locally administered, system-wide trust settings.

case system

System trust settings.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

