

- Quick Look UI
- QLPreviewView
-  previewItem 

Instance Property

# previewItem

The item to preview.

macOS 10.6+

``` source
@MainActor
var previewItem: (any QLPreviewItem)! { get set }
```

## Discussion

Quick Look requires Items you wish to conform to the QLPreviewItem protocol. When you set this property, the QLPreviewView loads the preview asynchronously. Due to this asynchronous behavior, don’t assume that the preview is ready immediately after assigning it to this property.

## See Also

### Displaying a Preview

func refreshPreviewItem()

Updates the preview to display the currently previewed item.

var displayState: Any!

The current display state of the previewItem.

var autostarts: Bool

A Boolean value that determines whether the preview starts automatically.

