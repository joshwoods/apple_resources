

- LiveCommunicationKit
- MergeConversationAction
-  init(conversationUUID:conversationUUIDToMergeWith:) 

Initializer

# init(conversationUUID:conversationUUIDToMergeWith:)

Created a new `MergeConversationAction`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
init(
    conversationUUID: UUID,
    conversationUUIDToMergeWith: UUID
)
```

## Parameters 

`conversationUUID`  

The unique identifier of the `Conversation` to which this action will apply.

`conversationUUIDToMergeWith`  

The unique identifier of the second `Conversation` that will be merged.

