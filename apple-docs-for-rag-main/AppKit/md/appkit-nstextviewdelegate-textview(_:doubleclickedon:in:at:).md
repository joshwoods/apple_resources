

- AppKit
- NSTextViewDelegate
-  textView(\_:doubleClickedOn:in:at:) 

Instance Method

# textView(\_:doubleClickedOn:in:at:)

Sent when the user double-clicks a cell.

macOS

``` source
@MainActor
optional func textView(
    _ textView: NSTextView,
    doubleClickedOn cell: any NSTextAttachmentCellProtocol,
    in cellFrame: NSRect,
    at charIndex: Int
)
```

## Parameters 

`textView`  

The text view sending the message.

`cell`  

The cell double-clicked by the user.

`cellFrame`  

The frame of the double-clicked cell.

`charIndex`  

The character index of the double-clicked cell.

## Discussion

The delegate can use this message as its cue to perform an action, such as opening the file represented by the attachment. `aTextView` is the first text view in a series shared by a layout manager, not necessarily the one that draws `cell`.

## See Also

### Clicking and Pasting

func textView(NSTextView, clickedOn: any NSTextAttachmentCellProtocol, in: NSRect, at: Int)

Sent when the user clicks a cell.

func textView(NSTextView, clickedOnLink: Any, at: Int) -> Bool

Sent after the user clicks a link.

