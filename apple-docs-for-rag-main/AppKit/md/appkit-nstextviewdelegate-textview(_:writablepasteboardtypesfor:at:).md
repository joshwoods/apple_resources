

- AppKit
- NSTextViewDelegate
-  textView(\_:writablePasteboardTypesFor:at:) 

Instance Method

# textView(\_:writablePasteboardTypesFor:at:)

Returns the writable pasteboard types for a given cell.

macOS

``` source
@MainActor
optional func textView(
    _ view: NSTextView,
    writablePasteboardTypesFor cell: any NSTextAttachmentCellProtocol,
    at charIndex: Int
) -> [NSPasteboard.PasteboardType]
```

## Parameters 

`view`  

The text view sending the message.

`cell`  

The cell in question.

`charIndex`  

The character index in the text view that was clicked.

## Return Value

An array of types that can be written to the pasteboard for `cell`.

## Discussion

This method is invoked after the user clicks `cell` at the specified `charIndex` location in `aTextView`. If the textView(_:draggedCell:in:event:at:) is not used, this method and textView(_:write:at:to:type:) allow `aTextView` to take care of attachment dragging and pasting, with the delegate responsible only for writing the attachment to the pasteboard.

## See Also

### Managing the Pasteboard

func textView(NSTextView, write: any NSTextAttachmentCellProtocol, at: Int, to: NSPasteboard, type: NSPasteboard.PasteboardType) -> Bool

Returns whether data of the specified type for the given cell could be written to the specified pasteboard.

