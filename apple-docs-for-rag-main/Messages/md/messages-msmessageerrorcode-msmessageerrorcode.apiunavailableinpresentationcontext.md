

- Messages
- MSMessageErrorCode
-  MSMessageErrorCode.apiUnavailableInPresentationContext 

Case

# MSMessageErrorCode.apiUnavailableInPresentationContext

The API is unavailable in the current context.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
case apiUnavailableInPresentationContext
```

## Mentioned in 

Adding Sticker packs and iMessage apps to the system Stickers app, Messages camera, and FaceTime

## Discussion

Different contexts may support only a subset of the Message framework API. For more information, see the MSMessagesAppViewController class’s presentationContext property and the MSMessagesAppPresentationContext.media constant.

## See Also

### Error Codes

case fileNotFound

The file could not be found.

case fileUnreadable

The file could not be read.

case improperFileType

The file is not a supported file type.

case improperFileURL

The URL does not refer to a local file.

case stickerFileImproperFileAttributes

The system cannot read one or more of the file’s attributes (for example, the file size).

case stickerFileImproperFileSize

The image used to create an MSSticker object is larger than 500 KB.

case stickerFileImproperFileFormat

The image used to create an MSSticker object is not one of the supported file types (PNG, APNG, GIF, or JPEG).

case urlExceedsMaxSize

The URL in an MSMessage object’s url property is longer than the maximum allowed length (5,000 characters).

case sendWhileNotVisible

A message was sent while the app was not visible.

case sendWithoutRecentInteraction

A message was sent, but the app has not registered a recent touch interaction from the user.

case unknown

An unexpected or unknown error has occurred.

