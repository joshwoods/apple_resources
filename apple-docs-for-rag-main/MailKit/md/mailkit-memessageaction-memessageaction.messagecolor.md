

- MailKit
- MEMessageAction
-  MEMessageAction.MessageColor 

Enumeration

# MEMessageAction.MessageColor

A color that the system uses to display a message in the message list.

macOS 12.0+

``` source
enum MessageColor
```

## Topics

### Specifying a Message Color

case green

Sets the color of the message to green.

case yellow

Sets the color of the message to yellow.

case orange

Sets the color of the message to orange.

case red

Sets the color of the message to red.

case purple

Sets the color of the message to purple.

case blue

Sets the color of the message to blue.

case gray

Sets the color of the message to gray.

case none

Clears the color of the message.

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

### Performing Actions on Messages

func decideAction(for: MEMessage, completionHandler: (MEMessageActionDecision?) -> Void)

Determines the action that the system takes when it downloads a message.

**Required**

class MEMessageAction

An action the system performs on a message, such as setting a color or archiving it.

class MEMessageActionDecision

The action that the system performs on a message, or a request to ask the action handler again later when the message content is available.

