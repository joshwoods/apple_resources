

- Messages
- MSMessagesAppPresentationContext
-  MSMessagesAppPresentationContext.media 

Case

# MSMessagesAppPresentationContext.media

A constant that indicates the iMessage app appears inside the Stickers app throughout iOS including in Messages, FaceTime, the emoji keyboard, and Markup.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
case media
```

## Mentioned in 

Adding Sticker packs and iMessage apps to the system Stickers app, Messages camera, and FaceTime

## Discussion

The media context supports only a subset of the Messages framework API. Specifically, the following limits apply:

- The iMessage app can only insert sticker and image attachments. You can’t insert MSMessage objects, text, or non-image assets.

- You can’t use any of the MSConversation class’s `send` messages (sendAttachment(_:withAlternateFilename:completionHandler:), send(_:completionHandler:), send(_:completionHandler:), or sendText(_:completionHandler:)).

- You can’t display a camera inside an MSMessagesAppPresentationContext.media context.

## See Also

### Presentation Contexts

case messages

A constant that indicates the iMessage app appears in Messages in the list of iMessage apps that appears when you press the plus button.

