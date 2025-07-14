

- LiveCommunicationKit
- ConversationManagerDelegate
-  conversationManager(\_:didDeactivate:) 

Instance Method

# conversationManager(\_:didDeactivate:)

Called when the provider’s audio session is deactivated.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
func conversationManager(
    _ manager: ConversationManager,
    didDeactivate audioSession: AVAudioSession
)
```

**Required**

## Parameters 

`manager`  

The `ConversationManager` that has requested the `ConversationAction` to be performed.

`audioSession`  

The audio session that was deactivated.

