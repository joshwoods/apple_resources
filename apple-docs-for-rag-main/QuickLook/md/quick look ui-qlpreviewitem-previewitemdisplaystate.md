

- Quick Look UI
- QLPreviewItem
-  previewItemDisplayState 

Instance Property

# previewItemDisplayState

The display state for the preview item.

macOS 10.6+

``` source
optional var previewItemDisplayState: Any! { get }
```

## Discussion

The display state is an opaque object used by the preview panel. You typically use the QLPreviewPanel method displayState to retrieve the display state which you save for later use in the preview item. This way you can preserve the display state when the panel moves from or to another controller.

This property is optional.

## See Also

### Instance Properties

var previewItemTitle: String!

The title to display for the preview item.

var previewItemURL: URL!

The URL of the item to preview.

**Required**

