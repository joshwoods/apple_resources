

- Quick Look
- QLPreviewControllerDataSource
-  numberOfPreviewItems(in:) 

Instance Method

# numberOfPreviewItems(in:)

Returns the number of preview items to include in the preview navigation list.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func numberOfPreviewItems(in controller: QLPreviewController) -> Int
```

**Required**

## Parameters 

`controller`  

The Quick Look preview controller that’s requesting the number of preview items.

## Return Value

The number of items that the Quick Look preview controller should include in its preview navigation list.

## Discussion

The system invokes this method to inform the preview controller of the number of preview items available.

If you push a Quick Look preview controller into view using a UINavigationController object that has a toolbar, the system automatically displays arrows in the toolbar to navigate among the items in the navigation list. If you’re not displaying a toolbar and want to provide your own method of switching among items, use the currentPreviewItemIndex property to indicate the item you want to display.

If you display a preview controller modally (full screen), the controller includes navigation arrows if there’s more than one item in the navigation list.

## See Also

### Providing data to a preview controller

func previewController(QLPreviewController, previewItemAt: Int) -> any QLPreviewItem

Returns the preview item that the controller displays for the specified index.

**Required**

