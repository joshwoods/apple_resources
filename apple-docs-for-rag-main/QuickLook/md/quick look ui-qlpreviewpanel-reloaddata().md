

- Quick Look UI
- QLPreviewPanel
-  reloadData() 

Instance Method

# reloadData()

Asks the preview panel to reload its data from its data source.

macOS 10.6+

``` source
@MainActor
func reloadData()
```

## Discussion

This method doesn’t refresh the visible item if it hasn’t changed.

## See Also

### Managing the Preview Items

var dataSource: (any QLPreviewPanelDataSource)!

The preview panel data source.

func refreshCurrentPreviewItem()

Asks the preview panel to recompute the preview of the current preview item.

var currentPreviewItemIndex: Int

The index of the current preview item.

var currentPreviewItem: (any QLPreviewItem)!

The currently previewed item.

var displayState: Any!

The preview panel’s display state.

