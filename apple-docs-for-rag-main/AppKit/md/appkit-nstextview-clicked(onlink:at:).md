

- AppKit
- NSTextView
-  clicked(onLink:at:) 

Instance Method

# clicked(onLink:at:)

Causes the text view to act as if the user clicked on some text with the given link as the value of a link attribute associated with the text.

macOS

``` source
@MainActor
func clicked(
    onLink link: Any,
    at charIndex: Int
)
```

## Parameters 

`link`  

The link that was clicked; the value of link.

`charIndex`  

The character index where the click occurred, indexed within the text storage.

## Discussion

If, for instance, you have a special attachment cell that can follow links, you can use this method to ask the text view to follow a link once you decide it should. In addition, this method is invoked by the text view during mouse tracking if the user clicks a link.

The `charIndex` parameter is a character index somewhere in the range of the link attribute. If the user actually physically clicked the link, then it should be the character that was originally clicked. In some cases a link may be opened indirectly or programmatically, in which case a character index somewhere in the range of the link attribute is supplied.

This method sends the textView(_:clickedOnLink:at:) delegate message if the delegate implements it, so that the delegate can handle the click.

## See Also

### Related Documentation

func textView(NSTextView, clickedOnLink: Any, at: Int) -> Bool

Sent after the user clicks a link.

### Clicking and pasting

func pasteAsPlainText(Any?)

Inserts the contents of the pasteboard into the receiver’s text as plain text.

func pasteAsRichText(Any?)

This action method inserts the contents of the pasteboard into the receiver’s text as rich text, maintaining its attributes.

