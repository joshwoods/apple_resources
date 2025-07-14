

- UIKit
- UITextInputDelegate
-  conversationContext(\_:didChange:) 

Instance Method

# conversationContext(\_:didChange:)

Tells the input delegate when text has changed in the input object for a conversation.

iOS 18.4+iPadOS 18.4+

``` source
@MainActor
func conversationContext(
    _ context: UIConversationContext?,
    didChange textInput: (any UITextInput)?
)
```

**Required**

## Mentioned in 

Adopting Smart Reply in your messaging or email app

