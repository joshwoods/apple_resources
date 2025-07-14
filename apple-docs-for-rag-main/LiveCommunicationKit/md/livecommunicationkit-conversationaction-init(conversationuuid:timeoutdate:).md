

- LiveCommunicationKit
- ConversationAction
-  init(conversationUUID:timeoutDate:) 

Initializer

# init(conversationUUID:timeoutDate:)

Initializes a new conversation action.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
convenience init(
    conversationUUID: UUID,
    timeoutDate: Date = Date(timeIntervalSinceNow: 30)
)
```

## Parameters 

`timeoutDate`  

The `Date` after which the action cannot be completed.

