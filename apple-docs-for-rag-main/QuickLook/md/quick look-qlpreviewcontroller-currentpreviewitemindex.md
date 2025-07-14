

- Quick Look
- QLPreviewController
-  currentPreviewItemIndex 

Instance Property

# currentPreviewItemIndex

The index within the preview item navigation list of the item displaying in the Quick Look preview controller.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var currentPreviewItemIndex: Int { get set }
```

## Discussion

You can change which item the preview controller displays, among those in a navigation list, by setting this property’s value. If the preview controller isn’t displaying an item, this property’s value is `NSNotFound`.

## See Also

### Managing item previews

class func canPreview(any QLPreviewItem) -> Bool

Returns a Boolean value that indicates whether the preview controller can display an item.

var currentPreviewItem: (any QLPreviewItem)?

The item displaying in the Quick Look preview controller.

func refreshCurrentPreviewItem()

Asks the Quick Look preview controller to recompute the display of the current preview item.

func reloadData()

Asks the preview controller to reload its data from its data source.

