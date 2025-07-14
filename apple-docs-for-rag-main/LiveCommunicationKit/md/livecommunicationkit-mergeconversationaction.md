

- LiveCommunicationKit
-  MergeConversationAction 

Class

# MergeConversationAction

This action is used to merge 2 separate `Conversation`s into 1.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
final class MergeConversationAction
```

## Topics

### Initializers

init(conversationUUID: UUID, conversationUUIDToMergeWith: UUID)

Created a new `MergeConversationAction`.

### Instance Properties

let conversationUUIDToMergeWith: UUID

The unique identifier of the second `Conversation` that will be merged.

## Relationships

### Inherits From

- ConversationAction

