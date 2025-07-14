

- LiveCommunicationKit
- ConversationManagerDelegate
-  conversationManager(\_:conversationChanged:) 

Instance Method

# conversationManager(\_:conversationChanged:)

Invoked when a `Conversation` is changed.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
func conversationManager(
    _ manager: ConversationManager,
    conversationChanged conversation: Conversation
)
```

**Required**

## Parameters 

`manager`  

The `ConversationManager` that issued the change.

`conversation`  

The `Conversation` that changed.

