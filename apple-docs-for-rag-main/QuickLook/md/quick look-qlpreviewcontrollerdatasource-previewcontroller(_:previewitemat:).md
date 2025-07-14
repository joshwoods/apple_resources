

- Quick Look
- QLPreviewControllerDataSource
-  previewController(\_:previewItemAt:) 

Instance Method

# previewController(\_:previewItemAt:)

Returns the preview item that the controller displays for the specified index.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func previewController(
    _ controller: QLPreviewController,
    previewItemAt index: Int
) -> any QLPreviewItem
```

**Required**

## Parameters 

`controller`  

The Quick Look preview controller that’s requesting a preview item.

`index`  

The index position, within the preview navigation list, of the item to preview.

## Return Value

The preview item to display. The item must be an `NSURL` object, or a custom object that conforms to the QLPreviewItem protocol.

## Discussion

The system invokes this method when the preview controller needs the preview item for a specified index position.

## See Also

### Providing data to a preview controller

func numberOfPreviewItems(in: QLPreviewController) -> Int

Returns the number of preview items to include in the preview navigation list.

**Required**

