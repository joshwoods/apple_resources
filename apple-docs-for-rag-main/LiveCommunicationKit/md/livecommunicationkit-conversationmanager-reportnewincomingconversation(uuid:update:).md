

- LiveCommunicationKit
- ConversationManager
-  reportNewIncomingConversation(uuid:update:) 

Instance Method

# reportNewIncomingConversation(uuid:update:)

Informs the system that there’s a new incoming Conversation, and the device should begin to ring and present the incoming Conversation UI.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
final func reportNewIncomingConversation(
    uuid: UUID,
    update: Conversation.Update
) async throws
```

## Parameters 

`uuid`  

The `UUID` used to identify the created Conversation.

`update`  

Optional fields used to configure the Conversation to an initial state.

