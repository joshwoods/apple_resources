

- Quick Look
- QLPreviewController
-  currentPreviewItem 

Instance Property

# currentPreviewItem

The item displaying in the Quick Look preview controller.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var currentPreviewItem: (any QLPreviewItem)? { get }
```

## Discussion

If the preview controller isn’t displaying an item, this property’s value is `nil`.

## See Also

### Managing item previews

class func canPreview(any QLPreviewItem) -> Bool

Returns a Boolean value that indicates whether the preview controller can display an item.

var currentPreviewItemIndex: Int

The index within the preview item navigation list of the item displaying in the Quick Look preview controller.

func refreshCurrentPreviewItem()

Asks the Quick Look preview controller to recompute the display of the current preview item.

func reloadData()

Asks the preview controller to reload its data from its data source.

