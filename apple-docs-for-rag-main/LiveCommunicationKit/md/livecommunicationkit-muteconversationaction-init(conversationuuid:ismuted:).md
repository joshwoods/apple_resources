

- LiveCommunicationKit
- MuteConversationAction
-  init(conversationUUID:isMuted:) 

Initializer

# init(conversationUUID:isMuted:)

Creates a new `MuteConversationAction`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
init(
    conversationUUID: UUID,
    isMuted: Bool
)
```

## Parameters 

`conversationUUID`  

The unique identfiier of the `Conversation` to which this action will be applied.

`isMuted`  

Specifies if the `Conversation` should be muted or unmuted upon execution of this action.

