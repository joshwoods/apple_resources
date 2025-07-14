

- LiveCommunicationKit
- PauseConversationAction
-  init(conversationUUID:isPaused:) 

Initializer

# init(conversationUUID:isPaused:)

Creates a new `PauseConversationAction`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
init(
    conversationUUID: UUID,
    isPaused: Bool
)
```

## Parameters 

`conversationUUID`  

The unique identfiier of the `Conversation` to which this action will be applied.

`isPaused`  

Specifies if the `Conversation` should be paused upon execution of this action.

