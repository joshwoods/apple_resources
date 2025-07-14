

- Quick Look
-  QLPreviewItemEditingMode 

Enumeration

# QLPreviewItemEditingMode

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum QLPreviewItemEditingMode
```

## Topics

### Enumeration Cases

case createCopy

case disabled

case updateContents

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Editing the content of a preview

func previewController(QLPreviewController, editingModeFor: any QLPreviewItem) -> QLPreviewItemEditingMode

Returns a value that indicates how the preview controller handles edits to the content of the previewed file.

func previewController(QLPreviewController, didUpdateContentsOf: any QLPreviewItem)

Tells the delegate that the content of a preview was updated successfully.

func previewController(QLPreviewController, didSaveEditedCopyOf: any QLPreviewItem, at: URL)

Tells the delegate that the preview item’s edited content was successfully saved to a copy at the given URL.

