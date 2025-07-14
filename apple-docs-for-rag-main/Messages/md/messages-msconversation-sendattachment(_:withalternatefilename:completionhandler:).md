

- Messages
- MSConversation
-  sendAttachment(\_:withAlternateFilename:completionHandler:) 

Instance Method

# sendAttachment(\_:withAlternateFilename:completionHandler:)

Sends the media file specified by the given URL.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
func sendAttachment(
    _ URL: URL,
    withAlternateFilename filename: String?,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func sendAttachment(
    _ URL: URL,
    withAlternateFilename filename: String?
) async throws
```

## Parameters 

`URL`  

A URL for the media file to send. This URL must refer to a file saved on the device.

`filename`  

An alternative name for the file. Use an alternative filename to better describe the attachment or to make the name more readable. If you pass a string, the Messages app uses the string as the attachment’s filename. If you pass `nil`, it parses the filename from the URL.

`completionHandler`  

A block that is called as soon as the message starts sending. This block is passed the following parameter:

error  
An error object. If an error occurred, this object contains information about the error; otherwise, it is set to `nil`. An error occurs if the user hasn’t recently interacted with your app.

## Mentioned in 

Adding Sticker packs and iMessage apps to the system Stickers app, Messages camera, and FaceTime

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func sendAttachment(_ URL: URL, withAlternateFilename filename: String?) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method starts sending the attachment automatically, without any additional user interactions. You can call this method only in response to a user action while in the MSMessagesAppPresentationContext.messages context.

When calling this method, the following rules apply:

- If the app is not visible, the send fails with a MSMessageErrorCode.sendWhileNotVisible error code.

- If the app has not registered a recent touch interaction from the user, the send fails with a MSMessageErrorCode.sendWithoutRecentInteraction error code.

- If the app is in the MSMessagesAppPresentationContext.media context, the send fails with an MSMessageErrorCode.apiUnavailableInPresentationContext error.

This method operates asynchronously. Although the method returns immediately, the actual work is deferred and performed in the background. As soon as the message starts to send, the system calls the completion block on a background queue.

## See Also

### Directly Sending a Message

func send(MSMessage, completionHandler: (((any Error)?) -> Void)?)

Sends a message object.

func send(MSSticker, completionHandler: (((any Error)?) -> Void)?)

Sends a sticker.

func sendText(String, completionHandler: (((any Error)?) -> Void)?)

Sends a text message.

