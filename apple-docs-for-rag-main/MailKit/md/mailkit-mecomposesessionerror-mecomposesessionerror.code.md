

- MailKit
- MEComposeSessionError
-  MEComposeSessionError.Code 

Enumeration

# MEComposeSessionError.Code

Errors that indicate invalid compose session states.

macOS 12.0+

``` source
enum Code
```

## Topics

### Indicating Erroneous States

case invalidBody

An error code that indicates the message’s body is invalid.

case invalidHeaders

An error code that indicates one or more of the message’s headers are invalid.

case invalidRecipients

An error code that indicates one or more of the message’s recipients are invalid.

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

### Enumerations

enum MEComposeUserAction

enum Flag

enum MEMessageEncryptionState

enum Code

