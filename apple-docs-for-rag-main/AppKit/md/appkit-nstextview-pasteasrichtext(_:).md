

- AppKit
- NSTextView
-  pasteAsRichText(\_:) 

Instance Method

# pasteAsRichText(\_:)

This action method inserts the contents of the pasteboard into the receiver’s text as rich text, maintaining its attributes.

macOS

``` source
@MainActor
func pasteAsRichText(_ sender: Any?)
```

## Parameters 

`sender`  

The control that sent the message; may be `nil`.

## Discussion

The text is inserted at the insertion point if there is one, otherwise replacing the selection.

## See Also

### Related Documentation

func insertText(Any)

Inserts `aString` into the receiver’s text at the insertion point if there is one, otherwise replacing the selection.

Deprecated

### Clicking and pasting

func clicked(onLink: Any, at: Int)

Causes the text view to act as if the user clicked on some text with the given link as the value of a link attribute associated with the text.

func pasteAsPlainText(Any?)

Inserts the contents of the pasteboard into the receiver’s text as plain text.

