

- LiveCommunicationKit
-  JoinConversationAction 

Class

# JoinConversationAction

Joins an incoming `Conversation` that may be currently ringing on the user’s device.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
final class JoinConversationAction
```

## Topics

### Initializers

init(conversationUUID: UUID)

Creates a new `JoinConversationAction`.

### Instance Methods

func fulfill(dateConnected: Date)

Indicates that the action has been successfully executed.

## Relationships

### Inherits From

- ConversationAction

