

- MailKit
-  MEComposeSessionError 

Structure

# MEComposeSessionError

An error that indicates the compose session is in an erroneous state.

macOS 12.0+

``` source
struct MEComposeSessionError
```

## Topics

### Indicating Erroneous States

static var invalidBody: MEComposeSessionError.Code

An error that indicates the message’s body is invalid.

static var invalidHeaders: MEComposeSessionError.Code

An error that indicates one or more of the message’s headers are invalid.

static var invalidRecipients: MEComposeSessionError.Code

An error that indicates one or more of the message’s recipients are invalid.

let MEComposeSessionErrorDomain: String

A constant for the compose session error domain.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Handling Compose Sessions

class MEComposeSession

An object that represents a single mail compose window.

func mailComposeSessionDidBegin(MEComposeSession)

Informs the handler when the user opens a compose window.

**Required**

func mailComposeSessionDidEnd(MEComposeSession)

Informs the handler when the user closes a compose window.

**Required**

