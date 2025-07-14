

- MailKit
-  MEMessageActionDecision 

Class

# MEMessageActionDecision

The action that the system performs on a message, or a request to ask the action handler again later when the message content is available.

macOS 12.0+

``` source
class MEMessageActionDecision
```

## Topics

### Determining Actions to Perform on Messages

class var invokeAgainWithBody: MEMessageActionDecision

An object that indicates the handler needs the message content before it can decide what action to take on a message.

### Type Methods

class func action(MEMessageAction) -> Self

class func actions([MEMessageAction]) -> Self

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

class MEMessageAction

An action the system performs on a message, such as setting a color or archiving it.

enum MessageColor

A color that the system uses to display a message in the message list.

