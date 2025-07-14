

- LiveCommunicationKit
- ConversationManager
-  reportConversationEvent(\_:for:) 

Instance Method

# reportConversationEvent(\_:for:)

Informs the system that some event has occurred and to update the given `Conversation` as needed.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
final func reportConversationEvent(
    _ event: Conversation.Event,
    for conversation: Conversation
)
```

## Parameters 

`event`  

The `Event` to be processed by the system.

`conversation`  

The `Conversation` to which the `Event` applies.

