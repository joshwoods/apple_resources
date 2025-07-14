

- Messages
- MSStickerView
-  init(frame:sticker:) 

Initializer

# init(frame:sticker:)

Initializes a new sticker view with the provided sticker and frame.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
init(
    frame: CGRect,
    sticker: MSSticker?
)
```

## Parameters 

`frame`  

A rectangular frame for the view, measured in points. The origin of the frame is relative to its superview. This method uses the provided rectangle to set the view’s center and bounds properties.

`sticker`  

The sticker object to be displayed. Pass `nil` to create an empty sticker view.

## Return Value

A newly initialized sticker view.

## Discussion

If the sticker image is larger than the view’s frame, the view scales down the sticker to fit. If the frame is larger than the sticker image, the view centers the image in the frame.

## See Also

### Working with Sticker Views

var sticker: MSSticker?

The displayed sticker object.

