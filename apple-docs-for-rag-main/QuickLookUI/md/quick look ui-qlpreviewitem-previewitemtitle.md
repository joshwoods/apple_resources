

- Quick Look UI
- QLPreviewItem
-  previewItemTitle 

Instance Property

# previewItemTitle

The title to display for the preview item.

macOS 10.6+

``` source
optional var previewItemTitle: String! { get }
```

## Discussion

If you don’t implement a getter method for this property, or if your method returns `nil`, Quick Look examines the URL or content of the previewed item to determine an appropriate title. Return a `non-nil` value for this property to provide a custom title.

## See Also

### Instance Properties

var previewItemDisplayState: Any!

The display state for the preview item.

var previewItemURL: URL!

The URL of the item to preview.

**Required**

