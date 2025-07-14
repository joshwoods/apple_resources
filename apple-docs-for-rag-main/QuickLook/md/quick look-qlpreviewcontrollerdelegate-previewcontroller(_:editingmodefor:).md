

- Quick Look
- QLPreviewControllerDelegate
-  previewController(\_:editingModeFor:) 

Instance Method

# previewController(\_:editingModeFor:)

Returns a value that indicates how the preview controller handles edits to the content of the previewed file.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func previewController(
    _ controller: QLPreviewController,
    editingModeFor previewItem: any QLPreviewItem
) -> QLPreviewItemEditingMode
```

## Parameters 

`controller`  

The controller that displays the preview.

`previewItem`  

The preview item for a file.

## Return Value

A value that indicates whether the previewed content is editable and how Quick Look saves the edits. If you return QLPreviewItemEditingMode.updateContents or QLPreviewItemEditingMode.createCopy to allow edits to a preview, make sure to implement the appropriate callbacks.

## Discussion

The platform invokes this callback when the preview controller loads its data. The system calls it for each preview item that it passes to the data source of the preview controller.

By default, a preview controller doesn’t allow edits to a preview. However, you can implement this method to allow the user to edit the previewed document, and specify the behavior for saving changes. The supported set of edits may change over time, but currently includes adding markup to images or PDFs, as well as simple edits to video files.

If you want to update the underlying file in place, return QLPreviewItemEditingMode.updateContents, and implement both the previewController(_:didUpdateContentsOf:) and previewController(_:didSaveEditedCopyOf:at:) delegate methods. The Quick Look feature calls previewController(_:didUpdateContentsOf:) first and updates the preview item’s content. If it can’t update the item directly, it invokes previewController(_:didSaveEditedCopyOf:at:) and creates a copy of the preview item’s content that contains the edits.

If you prefer to always save edits to a copy of the preview item’s content, return QLPreviewItemEditingMode.createCopy and implement previewController(_:didSaveEditedCopyOf:at:).

## See Also

### Editing the content of a preview

enum QLPreviewItemEditingMode

func previewController(QLPreviewController, didUpdateContentsOf: any QLPreviewItem)

Tells the delegate that the content of a preview was updated successfully.

func previewController(QLPreviewController, didSaveEditedCopyOf: any QLPreviewItem, at: URL)

Tells the delegate that the preview item’s edited content was successfully saved to a copy at the given URL.

