

- LiveCommunicationKit
- ConversationManagerDelegate
-  conversationManager(\_:didActivate:) 

Instance Method

# conversationManager(\_:didActivate:)

Called when the provider’s audio session is activated.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
func conversationManager(
    _ manager: ConversationManager,
    didActivate audioSession: AVAudioSession
)
```

**Required**

## Parameters 

`manager`  

The `ConversationManager` that has requested the `ConversationAction` to be performed.

`audioSession`  

The audio session that was activated.

