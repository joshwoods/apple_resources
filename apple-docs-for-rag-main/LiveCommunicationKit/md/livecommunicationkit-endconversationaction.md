

- LiveCommunicationKit
-  EndConversationAction 

Class

# EndConversationAction

Removes the local member from the specified `Conversation` and stops all audio/video streams, but doesn’t necessarily end the `Conversation` for remote members.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
final class EndConversationAction
```

## Topics

### Initializers

init(conversationUUID: UUID)

Creates a new `EndConversationAction`.

### Instance Methods

func fulfill(dateEnded: Date)

Indicates that the action has been successfully executed.

## Relationships

### Inherits From

- ConversationAction

