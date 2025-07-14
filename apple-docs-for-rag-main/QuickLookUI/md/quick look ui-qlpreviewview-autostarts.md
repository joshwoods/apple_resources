

- Quick Look UI
- QLPreviewView
-  autostarts 

Instance Property

# autostarts

A Boolean value that determines whether the preview starts automatically.

macOS 10.6+

``` source
@MainActor
var autostarts: Bool { get set }
```

## Discussion

Set this property to allow previews of movie files to start playback automatically when displayed.

## See Also

### Displaying a Preview

var previewItem: (any QLPreviewItem)!

The item to preview.

func refreshPreviewItem()

Updates the preview to display the currently previewed item.

var displayState: Any!

The current display state of the previewItem.

