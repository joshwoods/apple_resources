

- Messages
-  MSStickerBrowserViewDataSource 

Protocol

# MSStickerBrowserViewDataSource

The protocol for dynamically providing stickers to a browser view.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
protocol MSStickerBrowserViewDataSource : NSObjectProtocol
```

## Overview

To load its stickers, the MSStickerBrowserView class performs the following steps:

1.  The browser calls the data source’s numberOfStickers(in:) method to get the number of stickers.

2.  The browser repeatedly calls the data source’s stickerBrowserView(_:stickerAt:) method to load the individual stickers. Initially, the browser requests only enough stickers to fill the screen. The browser requests additional stickers as the user scrolls and new stickers become visible.

Both methods are required. If the sticker collection changes at runtime, call the MSStickerBrowserView class’s reloadData() method to reload the stickers.

## Topics

### Providing Stickers

func numberOfStickers(in: MSStickerBrowserView) -> Int

Asks the data source for the number of stickers that the browser will display.

**Required**

func stickerBrowserView(MSStickerBrowserView, stickerAt: Int) -> MSSticker

Asks the data source for the sticker object that the browser will display at the provided index.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- MSStickerBrowserViewController

## See Also

### Managing the Sticker Collection Contents

var dataSource: (any MSStickerBrowserViewDataSource)?

The sticker browser’s data source.

func reloadData()

Asks the sticker browser to reload its data from the data source.

