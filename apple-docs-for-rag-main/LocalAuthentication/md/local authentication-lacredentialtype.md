

- Local Authentication
-  LACredentialType 

Enumeration

# LACredentialType

The types of credentials to be used for authentication.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 3.0+

``` source
enum LACredentialType
```

## Topics

### Cases

case applicationPassword

Specifies that a password is provided by the application.

case smartCardPIN

### Constants

var kLACredentialTypeApplicationPassword: Int32

Specifies that a password is provided by the application.

var kLACredentialSmartCardPIN: Int32

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing credentials

func setCredential(Data?, type: LACredentialType) -> Bool

Sets an application-provided credential to be used when evaluating authentication.

func isCredentialSet(LACredentialType) -> Bool

Returns a Boolean value indicating whether the specified credential type is set.

