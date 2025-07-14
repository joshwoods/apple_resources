

- Messages
- MSStickerBrowserViewDataSource
-  numberOfStickers(in:) 

Instance Method

# numberOfStickers(in:)

Asks the data source for the number of stickers that the browser will display.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
func numberOfStickers(in stickerBrowserView: MSStickerBrowserView) -> Int
```

**Required**

## Parameters 

`stickerBrowserView`  

The sticker browser view that displays these stickers.

## Return Value

The number of stickers. This must be a non-negative number.

## See Also

### Providing Stickers

func stickerBrowserView(MSStickerBrowserView, stickerAt: Int) -> MSSticker

Asks the data source for the sticker object that the browser will display at the provided index.

**Required**

