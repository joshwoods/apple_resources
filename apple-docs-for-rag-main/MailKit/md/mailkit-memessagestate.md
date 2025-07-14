

- MailKit
-  MEMessageState 

Enumeration

# MEMessageState

The state of a message: sent, unsent, or received.

macOS 12.0+

``` source
enum MEMessageState
```

## Topics

### Determining Message State

case draft

A state that indicates the user is composing the message, and hasn’t sent it yet.

case received

A state that indicates the system has received and stored the message.

case sending

A state that indicates the system is in the process of sending the message.

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

### Message Properties

class MEMessage

An object that contains information about a mail message, such as the subject, addressees, date sent, and the message contents.

