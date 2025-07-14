

- Quick Look UI
- QLPreviewPanel
-  currentPreviewItem 

Instance Property

# currentPreviewItem

The currently previewed item.

macOS 10.6+

``` source
@MainActor
var currentPreviewItem: (any QLPreviewItem)! { get }
```

## Discussion

The value is `nil` if there’s no current preview item.

## See Also

### Managing the Preview Items

var dataSource: (any QLPreviewPanelDataSource)!

The preview panel data source.

func reloadData()

Asks the preview panel to reload its data from its data source.

func refreshCurrentPreviewItem()

Asks the preview panel to recompute the preview of the current preview item.

var currentPreviewItemIndex: Int

The index of the current preview item.

var displayState: Any!

The preview panel’s display state.

