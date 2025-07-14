

- AppKit
- NSTextViewDelegate
-  textView(\_:clickedOnLink:at:) 

Instance Method

# textView(\_:clickedOnLink:at:)

Sent after the user clicks a link.

macOS

``` source
@MainActor
optional func textView(
    _ textView: NSTextView,
    clickedOnLink link: Any,
    at charIndex: Int
) -> Bool
```

## Parameters 

`textView`  

The text view sending the message.

`link`  

The link that was clicked; the value of link.

`charIndex`  

The character index where the click occurred, indexed within the text storage.

## Return Value

true if the click was handled; otherwise, false to allow the next responder to handle it.

## Discussion

The delegate can use this method to handle the click on the link. It is invoked by clicked(onLink:at:).

The `charIndex` parameter is a character index somewhere in the range of the link attribute. If the user actually physically clicked the link, then it should be the character that was originally clicked. In some cases a link may be opened indirectly or programmatically, in which case a character index somewhere in the range of the link attribute is supplied.

## See Also

### Related Documentation

func clicked(onLink: Any, at: Int)

Causes the text view to act as if the user clicked on some text with the given link as the value of a link attribute associated with the text.

### Clicking and Pasting

func textView(NSTextView, clickedOn: any NSTextAttachmentCellProtocol, in: NSRect, at: Int)

Sent when the user clicks a cell.

func textView(NSTextView, doubleClickedOn: any NSTextAttachmentCellProtocol, in: NSRect, at: Int)

Sent when the user double-clicks a cell.

