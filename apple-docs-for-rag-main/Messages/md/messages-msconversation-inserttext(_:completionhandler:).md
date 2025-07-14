

- Messages
- MSConversation
-  insertText(\_:completionHandler:) 

Instance Method

# insertText(\_:completionHandler:)

Inserts text into the Messages app’s input field.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
func insertText(
    _ text: String,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func insertText(_ text: String) async throws
```

## Parameters 

`text`  

The text to be inserted.

`completionHandler`  

A block that is called as soon as the insertion is complete. This block is passed the following parameter:

error  
An error object. If an error occurred, this object contains information about the error; otherwise, it is set to `nil`.

## Mentioned in 

Adding Sticker packs and iMessage apps to the system Stickers app, Messages camera, and FaceTime

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func insertText(_ text: String) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Use this method to insert text into the Message app’s input field. Users can then send the text by tapping Send. iMessage apps suport this method only in the MSMessagesAppPresentationContext.messages context. If called in the MSMessagesAppPresentationContext.media context, the method fails with an MSMessageErrorCode.apiUnavailableInPresentationContext error.

This method operates asynchronously. Although the method returns immediately, the actual work is deferred and performed in the background. As soon as the attachment is inserted, the system calls the completion block on a background queue.

Note

This method does not send the text message. It inserts the text into the Messages app’s input field. The text is not sent until the user taps Send.

## See Also

### Inserting Content into the Input Field

func insertAttachment(URL, withAlternateFilename: String?, completionHandler: (((any Error)?) -> Void)?)

Inserts an attachment into the current context.

func insert(MSMessage, completionHandler: (((any Error)?) -> Void)?)

Inserts a message object into the Messages app’s input field.

func insert(MSSticker, completionHandler: (((any Error)?) -> Void)?)

Inserts a sticker into the current context.

