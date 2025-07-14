

- AppKit
- NSTextView
-  insertText(\_:) Deprecated

Instance Method

# insertText(\_:)

Inserts `aString` into the receiver’s text at the insertion point if there is one, otherwise replacing the selection.

macOS 10.0–10.11Deprecated

``` source
@MainActor
func insertText(_ insertString: Any)
```

Deprecated

Use `NSTextInputClient` method insertText(_:replacementRange:) instead.

## Parameters 

`insertString`  

The string to insert. `aString` can be either an NSString object or an NSAttributedString object.

## Discussion

The inserted text is assigned the current typing attributes.

This method is the means by which text typed by the user enters an NSTextView. See the NSInputManager class and NSTextInput protocol specifications for more information.

This method is the entry point for inserting text typed by the user and is generally not suitable for other purposes. Programmatic modification of the text is best done by operating on the text storage directly. Because this method pertains to the actions of the user, the text view must be editable for the insertion to work.

## See Also

### Related Documentation

var typingAttributes: [NSAttributedString.Key : Any]

The receiver’s typing attributes.

### Inserting text

var allowedInputSourceLocales: [String]?

An array of locale identifiers representing input sources that are allowed to be enabled when the receiver has the keyboard focus.

