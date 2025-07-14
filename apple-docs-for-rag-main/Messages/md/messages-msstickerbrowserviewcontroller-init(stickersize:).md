

- Messages
- MSStickerBrowserViewController
-  init(stickerSize:) 

Initializer

# init(stickerSize:)

Creates a new sticker browser view controller with stickers of the provided size.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
init(stickerSize: MSStickerSize)
```

## Parameters 

`stickerSize`  

A constant that indicates the size of the stickers. For a list of possible values, see MSStickerSize.

## Return Value

A newly instantiated sticker browser controller.

## See Also

### Working with Stickers

var stickerBrowserView: MSStickerBrowserView

The sticker browser view managed by this controller.

var stickerSize: MSStickerSize

A constant that indicates the size of the stickers.

