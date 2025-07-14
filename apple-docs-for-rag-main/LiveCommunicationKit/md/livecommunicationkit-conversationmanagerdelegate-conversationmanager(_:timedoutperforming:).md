

- LiveCommunicationKit
- ConversationManagerDelegate
-  conversationManager(\_:timedOutPerforming:) 

Instance Method

# conversationManager(\_:timedOutPerforming:)

Called when a `ConversationAction` is not performed before it expires.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
func conversationManager(
    _ manager: ConversationManager,
    timedOutPerforming action: ConversationAction
)
```

**Required**

## Parameters 

`manager`  

The `ConversationManager` that has requested the `ConversationAction` to be performed.

`action`  

The `ConversationAction` that timed out.

