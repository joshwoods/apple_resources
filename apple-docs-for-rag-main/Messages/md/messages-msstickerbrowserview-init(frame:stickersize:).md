

- Messages
- MSStickerBrowserView
-  init(frame:stickerSize:) 

Initializer

# init(frame:stickerSize:)

Creates a new sticker browser containing stickers of the specified size.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
init(
    frame: CGRect,
    stickerSize: MSStickerSize
)
```

## Parameters 

`frame`  

A rectangular frame for the view, measured in points. The origin of the frame is relative to its superview. This method uses the provided rectangle to set the view’s center and bounds properties.

`stickerSize`  

The size of the stickers. For a list of possible values, see MSStickerSize.

## Return Value

A newly initialized sticker browser view.

## See Also

### Creating Sticker Browser Views

init(frame: CGRect)

Creates a new sticker browser containing medium-sized stickers.

