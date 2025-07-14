

- MailKit
-  MEMessageAction 

Class

# MEMessageAction

An action the system performs on a message, such as setting a color or archiving it.

macOS 12.0+

``` source
class MEMessageAction
```

## Topics

### Changing the Read Status

class var markAsRead: MEMessageAction

An object that marks the message as read.

class var markAsUnread: MEMessageAction

An object that marks the message as unread.

### Transferring Messages

class var moveToArchive: MEMessageAction

An object that moves the message to the account’s Archive mailbox.

class var moveToJunk: MEMessageAction

An object that moves the message to the account’s Junk mailbox.

class var moveToTrash: MEMessageAction

An object that moves the message to the account’s Trash mailbox.

### Type Methods

class func flag(MEMessageAction.Flag) -> Self

class func setBackgroundColor(MEMessageAction.MessageColor) -> Self

### Enumerations

enum Flag

enum MessageColor

A color that the system uses to display a message in the message list.

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

### Performing Actions on Messages

func decideAction(for: MEMessage, completionHandler: (MEMessageActionDecision?) -> Void)

Determines the action that the system takes when it downloads a message.

**Required**

class MEMessageActionDecision

The action that the system performs on a message, or a request to ask the action handler again later when the message content is available.

enum MessageColor

A color that the system uses to display a message in the message list.

