

- LiveCommunicationKit
- ConversationManagerDelegate
-  conversationManager(\_:perform:) 

Instance Method

# conversationManager(\_:perform:)

Called when the system requires that some `ConversationAction` is performed.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
func conversationManager(
    _ manager: ConversationManager,
    perform action: ConversationAction
)
```

**Required**

## Parameters 

`manager`  

The `ConversationManager` that has requested the `ConversationAction` to be performed.

`action`  

The `ConversationAction` to be performed and fulfilled.

