

- MailKit
-  MEComposeSession 

Class

# MEComposeSession

An object that represents a single mail compose window.

macOS 12.0+

``` source
class MEComposeSession
```

## Topics

### Managing Compose Sessions

var sessionID: UUID

A unique identifier for the session.

func reload()

Refreshes the compose session with the extension’s new information.

### Accessing Message Properties

var mailMessage: MEMessage

The properties of the mail message, such as the subject and recipients.

### Instance Properties

var composeContext: MEComposeContext

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Handling Compose Sessions

func mailComposeSessionDidBegin(MEComposeSession)

Informs the handler when the user opens a compose window.

**Required**

func mailComposeSessionDidEnd(MEComposeSession)

Informs the handler when the user closes a compose window.

**Required**

struct MEComposeSessionError

An error that indicates the compose session is in an erroneous state.

