

- UIKit
- UITextInputTraits
-  conversationContext 

Instance Property

# conversationContext

A reference to a conversation, such as a mail or messaging thread.

iOS 18.4+iPadOS 18.4+

``` source
@MainActor
optional var conversationContext: UIConversationContext? { get set }
```

## Mentioned in 

Adopting Smart Reply in your messaging or email app

## Discussion

Set this conversation context before the keyboard appears; the keyboard uses this context to initialize its conversation context value. When updates occur in the conversation, call conversationContext(_:didChange:) on the `inputDelegate` property for UITextInput objects, such as UITextView/inputDelegate`or`UITextField/inputDelegate\`\`.

