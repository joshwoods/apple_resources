

- AppKit
- NSTextViewDelegate
-  textView(\_:clickedOn:in:at:) 

Instance Method

# textView(\_:clickedOn:in:at:)

Sent when the user clicks a cell.

macOS

``` source
@MainActor
optional func textView(
    _ textView: NSTextView,
    clickedOn cell: any NSTextAttachmentCellProtocol,
    in cellFrame: NSRect,
    at charIndex: Int
)
```

## Parameters 

`textView`  

The text view sending the message.

`cell`  

The cell clicked by the user.

`cellFrame`  

The frame of the clicked cell.

`charIndex`  

The character index of the clicked cell.

## Discussion

The delegate can use this message as its cue to perform an action or select the attachment cell’s character. `aTextView` is the first text view in a series shared by a layout manager, not necessarily the one that draws `cell`.

The delegate may subsequently receive a textView(_:doubleClickedOn:in:at:) message if the user continues to perform a double click.

## See Also

### Clicking and Pasting

func textView(NSTextView, doubleClickedOn: any NSTextAttachmentCellProtocol, in: NSRect, at: Int)

Sent when the user double-clicks a cell.

func textView(NSTextView, clickedOnLink: Any, at: Int) -> Bool

Sent after the user clicks a link.

