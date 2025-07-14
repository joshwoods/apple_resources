

- AppKit
- NSTextViewDelegate
-  textView(\_:draggedCell:in:event:at:) 

Instance Method

# textView(\_:draggedCell:in:event:at:)

Sent when the user attempts to drag a cell.

macOS

``` source
@MainActor
optional func textView(
    _ view: NSTextView,
    draggedCell cell: any NSTextAttachmentCellProtocol,
    in rect: NSRect,
    event: NSEvent,
    at charIndex: Int
)
```

## Parameters 

`view`  

The text view sending the message.

`cell`  

The cell being dragged.

`rect`  

The rectangle from which the cell was dragged.

`event`  

The mouse-down event that preceded the mouse-dragged event.

`charIndex`  

The character position where the mouse button was clicked.

## Discussion

The delegate can use this message as its cue to initiate a dragging operation.

## See Also

### Related Documentation

func dragFile(String, from: NSRect, slideBack: Bool, event: NSEvent) -> Bool

Initiates a dragging operation from the view, allowing the user to drag a file icon to any application that has window or view objects that accept files.

Deprecated

