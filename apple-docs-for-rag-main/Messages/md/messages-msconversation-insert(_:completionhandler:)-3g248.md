

- Messages
- MSConversation
-  insert(\_:completionHandler:) 

Instance Method

# insert(\_:completionHandler:)

Inserts a message object into the Messages app’s input field.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
func insert(
    _ message: MSMessage,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func insert(_ message: MSMessage) async throws
```

## Parameters 

`message`  

The message object to be inserted.

`completionHandler`  

A block that is called as soon as the insertion is complete. This block is passed the following parameter:

error  
An error object. If an error occurred, this object contains information about the error; otherwise, it is set to `nil`. The system validates the message before inserting it. Errors occur if the message is invalid. Otherwise, the message is inserted into the Messages app’s input field.

## Mentioned in 

Adding Sticker packs and iMessage apps to the system Stickers app, Messages camera, and FaceTime

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func insert(_ message: MSMessage) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Use this method to insert an MSMessage object into the Message app’s input field. Users can then send the message by tapping Send. iMessage apps suport this method only in the MSMessagesAppPresentationContext.messages context. If called in the MSMessagesAppPresentationContext.media context, the method fails with an MSMessageErrorCode.apiUnavailableInPresentationContext error.

The message object’s appearance is determined by its layout property. The message can contain app-specific data and can be associated with a session, letting other participants update the message. For more information, see MSMessage.

This method operates asynchronously. Although the method returns immediately, the actual work is deferred and performed in the background. As soon as the attachment is inserted, the system calls the completion block on a background queue.

Note

This method does not send the message. It inserts the message into the Messages app’s input field. The message is not sent until the user taps Send.

Subsequent calls to this method replace any existing message in the input field.

If the message was initialized using the session from an existing message, a new message is not added to the transcript. Instead, the system takes the following steps as soon as the user sends the message:

1.  The system moves the existing message to the bottom of the conversation transcript.

2.  It updates the message with the new content.

## See Also

### Inserting Content into the Input Field

func insertAttachment(URL, withAlternateFilename: String?, completionHandler: (((any Error)?) -> Void)?)

Inserts an attachment into the current context.

func insert(MSSticker, completionHandler: (((any Error)?) -> Void)?)

Inserts a sticker into the current context.

func insertText(String, completionHandler: (((any Error)?) -> Void)?)

Inserts text into the Messages app’s input field.

