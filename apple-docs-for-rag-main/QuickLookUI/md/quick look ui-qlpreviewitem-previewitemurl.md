

- Quick Look UI
- QLPreviewItem
-  previewItemURL 

Instance Property

# previewItemURL

The URL of the item to preview.

macOS 10.6+

``` source
var previewItemURL: URL! { get }
```

**Required**

## Discussion

QLPreviewController uses this property to get an item’s URL. In typical use, you’d implement a getter method in your preview item class to provide this value.

The value of this property must be a file-type URL.

If the item isn’t available for preview, this property’s getter method should return `nil`. In this case, the QLPreviewController displays a “loading” view. Use refreshCurrentPreviewItem() to reload the item once the URL content is available.

## See Also

### Instance Properties

var previewItemDisplayState: Any!

The display state for the preview item.

var previewItemTitle: String!

The title to display for the preview item.

