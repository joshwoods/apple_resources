

- Messages
- MSStickerBrowserView
-  reloadData() 

Instance Method

# reloadData()

Asks the sticker browser to reload its data from the data source.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
func reloadData()
```

## See Also

### Managing the Sticker Collection Contents

var dataSource: (any MSStickerBrowserViewDataSource)?

The sticker browser’s data source.

protocol MSStickerBrowserViewDataSource

The protocol for dynamically providing stickers to a browser view.

