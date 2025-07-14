

- Quick Look
- QLPreviewController
-  canPreview(\_:) 

Type Method

# canPreview(\_:)

Returns a Boolean value that indicates whether the preview controller can display an item.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

**iOS, iPadOS, visionOS**

``` source
@MainActor
class func canPreview(_ item: any QLPreviewItem) -> Bool
```

**Mac Catalyst**

``` source
@MainActor
class func canPreviewItem(_ item: any QLPreviewItem) -> Bool
```

## Parameters 

`item`  

An item to preview.

## Return Value

Returns true if the Quick Look preview controller can display the specified preview item.

## Discussion

If the system can’t display an item, but you still attempt to display it, a Quick Look preview controller displays a generic error. Always check whether you can display an item before choosing to do so.

For supported file types, see QLPreviewController.

## See Also

### Managing item previews

var currentPreviewItem: (any QLPreviewItem)?

The item displaying in the Quick Look preview controller.

var currentPreviewItemIndex: Int

The index within the preview item navigation list of the item displaying in the Quick Look preview controller.

func refreshCurrentPreviewItem()

Asks the Quick Look preview controller to recompute the display of the current preview item.

func reloadData()

Asks the preview controller to reload its data from its data source.

