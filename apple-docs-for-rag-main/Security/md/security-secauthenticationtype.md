

- Security
-  SecAuthenticationType 

Enumeration

# SecAuthenticationType

The authentication type to use for an Internet password.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum SecAuthenticationType
```

## Topics

### Constants

case NTLM

Specifies Windows NT LAN Manager authentication.

case MSN

Specifies Microsoft Network default authentication.

case DPA

Specifies Distributed Password authentication.

case RPA

Specifies Remote Password authentication.

case httpBasic

Specifies HTTP Basic authentication.

case httpDigest

Specifies HTTP Digest Access authentication.

case htmlForm

Specifies HTML form based authentication.

case `default`

Specifies the default authentication type.

case any

Specifies that any authentication type is acceptable.

### Initializers

init?(rawValue: FourCharCode)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

