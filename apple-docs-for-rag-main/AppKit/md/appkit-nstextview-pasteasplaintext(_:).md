

- AppKit
- NSTextView
-  pasteAsPlainText(\_:) 

Instance Method

# pasteAsPlainText(\_:)

Inserts the contents of the pasteboard into the receiver’s text as plain text.

macOS

``` source
@MainActor
func pasteAsPlainText(_ sender: Any?)
```

## Parameters 

`sender`  

The control that sent the message; may be `nil`.

## Discussion

This method behaves analogously to insertText(_:).

## See Also

### Related Documentation

func insertText(Any)

Inserts `aString` into the receiver’s text at the insertion point if there is one, otherwise replacing the selection.

Deprecated

### Clicking and pasting

func clicked(onLink: Any, at: Int)

Causes the text view to act as if the user clicked on some text with the given link as the value of a link attribute associated with the text.

func pasteAsRichText(Any?)

This action method inserts the contents of the pasteboard into the receiver’s text as rich text, maintaining its attributes.

