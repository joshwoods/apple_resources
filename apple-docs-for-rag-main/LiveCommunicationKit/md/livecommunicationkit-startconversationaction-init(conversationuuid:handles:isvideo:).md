

- LiveCommunicationKit
- StartConversationAction
-  init(conversationUUID:handles:isVideo:) 

Initializer

# init(conversationUUID:handles:isVideo:)

Creates a new `StartConversationAction`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
init(
    conversationUUID: UUID,
    handles: [Handle],
    isVideo: Bool
)
```

## Parameters 

`conversationUUID`  

The unique identfiier of the `Conversation` to which this action will be applied.

`handles`  

The `Handle`s of all remote members who will be invited to join the `Conversation`.

`isVideo`  

Specifies if the `Conversation` contains a video stream.

