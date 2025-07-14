

- Quick Look
- QLPreviewControllerDelegate
-  previewController(\_:didUpdateContentsOf:) 

Instance Method

# previewController(\_:didUpdateContentsOf:)

Tells the delegate that the content of a preview was updated successfully.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func previewController(
    _ controller: QLPreviewController,
    didUpdateContentsOf previewItem: any QLPreviewItem
)
```

## Parameters 

`controller`  

The controller that displays the preview.

`previewItem`  

The preview item for a file.

## Discussion

The platform invokes this callback after the preview controller successfully overwrites the file at the `previewItem’`s previewItemURL with an updated file.

The platform may invoke the callback multiple times consecutively with the successive edited versions of the preview item. It typically invokes the callback once for each time the user saves their edits.

## See Also

### Editing the content of a preview

func previewController(QLPreviewController, editingModeFor: any QLPreviewItem) -> QLPreviewItemEditingMode

Returns a value that indicates how the preview controller handles edits to the content of the previewed file.

enum QLPreviewItemEditingMode

func previewController(QLPreviewController, didSaveEditedCopyOf: any QLPreviewItem, at: URL)

Tells the delegate that the preview item’s edited content was successfully saved to a copy at the given URL.

