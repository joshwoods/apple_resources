

- LiveCommunicationKit
-  StartConversationAction 

Class

# StartConversationAction

Starts an outgoing `Conversation` that will ring on remote member’s devices.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
final class StartConversationAction
```

## Topics

### Initializers

init(conversationUUID: UUID, handles: [Handle], isVideo: Bool)

Creates a new `StartConversationAction`.

### Instance Properties

let handles: [Handle]

The `Handle`s of all remote members who will be invited to join the `Conversation`.

let isVideo: Bool

Specifies if the `Conversation` contains a video stream.

### Instance Methods

func fulfill(dateStarted: Date)

Indicates that the action has been successfully executed.

## Relationships

### Inherits From

- ConversationAction

