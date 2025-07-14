

- Messages
- MSConversation
-  send(\_:completionHandler:) 

Instance Method

# send(\_:completionHandler:)

Sends a message object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
func send(
    _ message: MSMessage,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func send(_ message: MSMessage) async throws
```

## Parameters 

`message`  

The message object to send.

`completionHandler`  

A block that’s called as soon as the message starts sending. This block is passed the following parameter:

error  
An error object. If an error occurred, this object contains information about the error; otherwise, it’s set to `nil`. The system validates the message before inserting it. Errors occur if the message is invalid or if the user hasn’t recently interacted with your app.

## Mentioned in 

Adding Sticker packs and iMessage apps to the system Stickers app, Messages camera, and FaceTime

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func send(_ message: MSMessage) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method starts sending the message object automatically, without any additional user interactions. You can call this method only in response to a user action while in the MSMessagesAppPresentationContext.messages context.

When calling this method, the following rules apply:

- If the app isn’t visible, the send fails with a MSMessageErrorCode.sendWhileNotVisible error code.

- If the app hasn’t registered a recent touch interaction from the user, the send fails with a MSMessageErrorCode.sendWithoutRecentInteraction error code.

- If the app is in the MSMessagesAppPresentationContext.media context, the send fails with an MSMessageErrorCode.apiUnavailableInPresentationContext error.

This method operates asynchronously. Although the method returns immediately, the actual work is deferred and performed in the background. As soon as the message starts to send, the system calls the completion block on a background queue.

Subsequent calls to this method replace any existing message in the input field.

If the message was initialized using the session from an existing message, a new message isn’t added to the transcript. Instead, the system takes the following steps as soon as the user sends the message:

1.  The system moves the existing message to the bottom of the conversation transcript.

2.  It updates the message with the new content.

## See Also

### Directly Sending a Message

func sendAttachment(URL, withAlternateFilename: String?, completionHandler: (((any Error)?) -> Void)?)

Sends the media file specified by the given URL.

func send(MSSticker, completionHandler: (((any Error)?) -> Void)?)

Sends a sticker.

func sendText(String, completionHandler: (((any Error)?) -> Void)?)

Sends a text message.

