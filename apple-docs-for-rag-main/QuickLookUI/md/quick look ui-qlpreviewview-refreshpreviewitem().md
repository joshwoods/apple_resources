

- Quick Look UI
- QLPreviewView
-  refreshPreviewItem() 

Instance Method

# refreshPreviewItem()

Updates the preview to display the currently previewed item.

macOS 10.6+

``` source
@MainActor
func refreshPreviewItem()
```

## Discussion

When you modify the object that the previewItem property points to, call this method to generate and display the new preview.

## See Also

### Displaying a Preview

var previewItem: (any QLPreviewItem)!

The item to preview.

var displayState: Any!

The current display state of the previewItem.

var autostarts: Bool

A Boolean value that determines whether the preview starts automatically.

