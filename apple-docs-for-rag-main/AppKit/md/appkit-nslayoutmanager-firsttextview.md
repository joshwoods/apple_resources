

- AppKit
- NSLayoutManager
-  firstTextView 

Instance Property

# firstTextView

The first text view in the layout manager’s series of text views.

macOS

``` source
unowned(unsafe) var firstTextView: NSTextView? { get }
```

## Discussion

This `NSTextView` object is the recipient of various `NSText` and `NSTextView` notifications.

## See Also

### Managing the responder chain

func layoutManagerOwnsFirstResponder(in: NSWindow) -> Bool

Indicates whether the first responder in the specified window is a text view for the layout manager.

var textViewForBeginningOfSelection: NSTextView?

The text view that contains the first glyph in the selection.

