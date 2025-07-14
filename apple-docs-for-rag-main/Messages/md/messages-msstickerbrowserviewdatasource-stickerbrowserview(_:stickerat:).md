

- Messages
- MSStickerBrowserViewDataSource
-  stickerBrowserView(\_:stickerAt:) 

Instance Method

# stickerBrowserView(\_:stickerAt:)

Asks the data source for the sticker object that the browser will display at the provided index.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
func stickerBrowserView(
    _ stickerBrowserView: MSStickerBrowserView,
    stickerAt index: Int
) -> MSSticker
```

**Required**

## Parameters 

`stickerBrowserView`  

The sticker browser view that displays these stickers.

`index`  

The index of the desired sticker.

## Return Value

A valid sticker object.

## Discussion

Do not perform any time-intensive activities in this method. For example, creating a sticker from a local image file should be fine, but you can’t download an image for your sticker.

## See Also

### Providing Stickers

func numberOfStickers(in: MSStickerBrowserView) -> Int

Asks the data source for the number of stickers that the browser will display.

**Required**

