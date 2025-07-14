

- Quick Look UI
- QLPreviewPanel
-  currentPreviewItemIndex 

Instance Property

# currentPreviewItemIndex

The index of the current preview item.

macOS 10.6+

``` source
@MainActor
var currentPreviewItemIndex: Int { get set }
```

## Discussion

The value is `NSNotFound` if there’s no current preview item.

## See Also

### Managing the Preview Items

var dataSource: (any QLPreviewPanelDataSource)!

The preview panel data source.

func reloadData()

Asks the preview panel to reload its data from its data source.

func refreshCurrentPreviewItem()

Asks the preview panel to recompute the preview of the current preview item.

var currentPreviewItem: (any QLPreviewItem)!

The currently previewed item.

var displayState: Any!

The preview panel’s display state.

