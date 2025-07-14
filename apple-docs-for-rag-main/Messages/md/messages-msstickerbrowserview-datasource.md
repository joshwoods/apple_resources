

- Messages
- MSStickerBrowserView
-  dataSource 

Instance Property

# dataSource

The sticker browser’s data source.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
weak var dataSource: (any MSStickerBrowserViewDataSource)? { get set }
```

## Discussion

If you are using an MSStickerBrowserViewController object, the controller automatically sets itself as the data source for the sticker browser view that it provides. If you instantiate and display your own sticker browser view, this property defaults to `nil`, and you must assign a data source.

## See Also

### Managing the Sticker Collection Contents

protocol MSStickerBrowserViewDataSource

The protocol for dynamically providing stickers to a browser view.

func reloadData()

Asks the sticker browser to reload its data from the data source.

