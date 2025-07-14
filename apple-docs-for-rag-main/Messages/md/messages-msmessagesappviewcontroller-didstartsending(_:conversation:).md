

- Messages
- MSMessagesAppViewController
-  didStartSending(\_:conversation:) 

Instance Method

# didStartSending(\_:conversation:)

Invoked when the user sends a message object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
func didStartSending(
    _ message: MSMessage,
    conversation: MSConversation
)
```

## Parameters 

`message`  

The message being sent.

`conversation`  

The conversation that the user is currently viewing in the Messages app.

## Mentioned in 

Adding Sticker packs and iMessage apps to the system Stickers app, Messages camera, and FaceTime

## Discussion

Override this method to respond when the user sends an MSMessage object. This method is called if you use the conversation’s insert(_:completionHandler:) method to add an MSMessage object to the Messages app’s input field, and the user taps Send. It does not guarantee that the message will be successfully sent or delivered.

The system does not call this method if the controller’s presentationStyle property is MSMessagesAppPresentationStyle.transcript, or if its presentationContext property is MSMessagesAppPresentationContext.media.

## See Also

### Tracking Messages

func willSelect(MSMessage, conversation: MSConversation)

Invoked in response to the user selecting a message object in the transcript, before the system updates the conversation’s selectedMessage property.

func didSelect(MSMessage, conversation: MSConversation)

Invoked in response to the user selecting a message object in the transcript, after the system updates the conversation’s selectedMessage property.

func didReceive(MSMessage, conversation: MSConversation)

Invoked when the iMessage app receives a new message object.

func didCancelSending(MSMessage, conversation: MSConversation)

Invoked when the user deletes a message object from the Messages app’s input field.

