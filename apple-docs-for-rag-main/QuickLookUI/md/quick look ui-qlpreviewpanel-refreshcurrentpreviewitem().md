

- Quick Look UI
- QLPreviewPanel
-  refreshCurrentPreviewItem() 

Instance Method

# refreshCurrentPreviewItem()

Asks the preview panel to recompute the preview of the current preview item.

macOS 10.6+

``` source
@MainActor
func refreshCurrentPreviewItem()
```

## See Also

### Managing the Preview Items

var dataSource: (any QLPreviewPanelDataSource)!

The preview panel data source.

func reloadData()

Asks the preview panel to reload its data from its data source.

var currentPreviewItemIndex: Int

The index of the current preview item.

var currentPreviewItem: (any QLPreviewItem)!

The currently previewed item.

var displayState: Any!

The preview panel’s display state.

