

- Quick Look
- QLPreviewController
-  reloadData() 

Instance Method

# reloadData()

Asks the preview controller to reload its data from its data source.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func reloadData()
```

## Discussion

Quick Look recomputes the displayed data only if the current preview item changes.

## See Also

### Managing item previews

class func canPreview(any QLPreviewItem) -> Bool

Returns a Boolean value that indicates whether the preview controller can display an item.

var currentPreviewItem: (any QLPreviewItem)?

The item displaying in the Quick Look preview controller.

var currentPreviewItemIndex: Int

The index within the preview item navigation list of the item displaying in the Quick Look preview controller.

func refreshCurrentPreviewItem()

Asks the Quick Look preview controller to recompute the display of the current preview item.

