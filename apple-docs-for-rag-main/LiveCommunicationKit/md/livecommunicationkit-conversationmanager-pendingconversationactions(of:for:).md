

- LiveCommunicationKit
- ConversationManager
-  pendingConversationActions(of:for:) 

Instance Method

# pendingConversationActions(of:for:)

Returns all pending `ConversationAction`s of the specified class for the specified call identifier that are incomplete.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
final func pendingConversationActions(
    of conversationActionClass: ConversationAction.Type,
    for conversation: Conversation
) -> [ConversationAction]
```

## Parameters 

`conversationActionClass`  

The desired `ConversationAction` subclass of actions to return.

`conversation`  

The desired `Conversation` for returned actions.

## Return Value

An array of call actions of the specified class for the specified `Conversation`.

