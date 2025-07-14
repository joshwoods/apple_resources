

- AppKit
- NSTextViewDelegate
-  textView(\_:write:at:to:type:) 

Instance Method

# textView(\_:write:at:to:type:)

Returns whether data of the specified type for the given cell could be written to the specified pasteboard.

macOS

``` source
@MainActor
optional func textView(
    _ view: NSTextView,
    write cell: any NSTextAttachmentCellProtocol,
    at charIndex: Int,
    to pboard: NSPasteboard,
    type: NSPasteboard.PasteboardType
) -> Bool
```

## Parameters 

`view`  

The text view sending the message.

`cell`  

The cell whose contents should be written to the pasteboard.

`charIndex`  

The index at which the cell was accessed.

`pboard`  

The pasteboard to which the cell’s contents should be written.

`type`  

The type of data that should be written.

## Return Value

true if the write succeeded, false otherwise.

## Discussion

The receiver should attempt to write the `cell` to `pboard` with the given `type`, and return success or failure.

## See Also

### Managing the Pasteboard

func textView(NSTextView, writablePasteboardTypesFor: any NSTextAttachmentCellProtocol, at: Int) -> [NSPasteboard.PasteboardType]

Returns the writable pasteboard types for a given cell.

