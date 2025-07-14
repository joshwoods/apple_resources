

- Quick Look UI
- QLPreviewView
-  displayState 

Instance Property

# displayState

The current display state of the previewItem.

macOS 10.6+

``` source
@MainActor
var displayState: Any! { get set }
```

## Discussion

This property is an opaque object that Quick Look uses to get and set the current display state of the preview. The display state could be, for example, the currently displayed page, the zoom factor on an image, or the position in a movie.

You can use this property to get and save the current display state of the preview before switching to another. This saving allows you to restore a preview later on when the user switches back to it.

## See Also

### Displaying a Preview

var previewItem: (any QLPreviewItem)!

The item to preview.

func refreshPreviewItem()

Updates the preview to display the currently previewed item.

var autostarts: Bool

A Boolean value that determines whether the preview starts automatically.

