

- Quick Look UI
- QLPreviewPanel
-  dataSource 

Instance Property

# dataSource

The preview panel data source.

macOS 10.6+

``` source
@MainActor
unowned(unsafe) var dataSource: (any QLPreviewPanelDataSource)! { get set }
```

## See Also

### Managing the Preview Items

func reloadData()

Asks the preview panel to reload its data from its data source.

func refreshCurrentPreviewItem()

Asks the preview panel to recompute the preview of the current preview item.

var currentPreviewItemIndex: Int

The index of the current preview item.

var currentPreviewItem: (any QLPreviewItem)!

The currently previewed item.

var displayState: Any!

The preview panel’s display state.

