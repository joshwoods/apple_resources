

- Messages
- MSMessagesAppViewController
-  didSelect(\_:conversation:) 

Instance Method

# didSelect(\_:conversation:)

Invoked in response to the user selecting a message object in the transcript, after the system updates the conversation’s selectedMessage property.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
func didSelect(
    _ message: MSMessage,
    conversation: MSConversation
)
```

## Parameters 

`message`  

The message selected by the user.

`conversation`  

The current conversation.

## Mentioned in 

Adding Sticker packs and iMessage apps to the system Stickers app, Messages camera, and FaceTime

## Discussion

This method is called when the user selects one of your app’s message objects in the transcript while your extension is active. Both the `message` parameter and the `conversation` object’s selectedMessage property contain the message selected by the user.

If you need to access the previously selected message, override the willSelect(_:conversation:) method instead.

This method is called when a new message arrives while your extension is active. You receive notifications about messages sent using your extension only. You cannot interact with messages from other extensions.

The system does not call this method if the controller’s presentationStyle property is MSMessagesAppPresentationStyle.transcript, or if its presentationContext property is MSMessagesAppPresentationContext.media.

## See Also

### Tracking Messages

func willSelect(MSMessage, conversation: MSConversation)

Invoked in response to the user selecting a message object in the transcript, before the system updates the conversation’s selectedMessage property.

func didReceive(MSMessage, conversation: MSConversation)

Invoked when the iMessage app receives a new message object.

func didStartSending(MSMessage, conversation: MSConversation)

Invoked when the user sends a message object.

func didCancelSending(MSMessage, conversation: MSConversation)

Invoked when the user deletes a message object from the Messages app’s input field.

