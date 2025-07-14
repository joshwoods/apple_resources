

- LiveCommunicationKit
-  PauseConversationAction 

Class

# PauseConversationAction

Pauses or unpauses a `Conversation`. Pausing a `Conversation` will stop all audio/video streams that apply to that `Conversation`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
final class PauseConversationAction
```

## Topics

### Initializers

init(conversationUUID: UUID, isPaused: Bool)

Creates a new `PauseConversationAction`.

### Instance Properties

let isPaused: Bool

Specifies if the `Conversation` should be paused upon execution of this action.

## Relationships

### Inherits From

- ConversationAction

