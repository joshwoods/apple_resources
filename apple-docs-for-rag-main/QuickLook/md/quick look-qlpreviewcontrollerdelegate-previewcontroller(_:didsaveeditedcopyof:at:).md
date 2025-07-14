

- Quick Look
- QLPreviewControllerDelegate
-  previewController(\_:didSaveEditedCopyOf:at:) 

Instance Method

# previewController(\_:didSaveEditedCopyOf:at:)

Tells the delegate that the preview item’s edited content was successfully saved to a copy at the given URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func previewController(
    _ controller: QLPreviewController,
    didSaveEditedCopyOf previewItem: any QLPreviewItem,
    at modifiedContentsURL: URL
)
```

## Parameters 

`controller`  

The controller that displays the preview.

`previewItem`  

The preview item for a file.

`modifiedContentsURL`  

A URL pointing to a temporary file that contains the edited version of the previewed file.

## Discussion

The platform invokes this callback with an edited copy of the preview item at `modifiedContentsURL`. It invokes the callback in the following scenarios:

- The editing mode of the `previewItem` is QLPreviewItemEditingMode.createCopy.

- The editing mode of the `previewItem` is QLPreviewItemEditingMode.updateContents and the system can’t overwrite its previewItemURL. In this case, `modifiedContentsURL` points to a temporary file on disk containing the edited copy.

- The editing mode of the preview item is QLPreviewItemEditingMode.updateContents and its content type doesn’t match the content type of the edited version. This mismatch means that the file type of the file at `modifiedContentsURL` may be different from the file type of the preview item.

The platform may invoke the callback multiple times consecutively with the successive edited versions of the preview item. It typically invokes the callback once for each time the user saves their edits.

## See Also

### Editing the content of a preview

func previewController(QLPreviewController, editingModeFor: any QLPreviewItem) -> QLPreviewItemEditingMode

Returns a value that indicates how the preview controller handles edits to the content of the previewed file.

enum QLPreviewItemEditingMode

func previewController(QLPreviewController, didUpdateContentsOf: any QLPreviewItem)

Tells the delegate that the content of a preview was updated successfully.

