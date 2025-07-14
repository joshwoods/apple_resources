

- AppKit
- NSLayoutManager
-  textViewForBeginningOfSelection 

Instance Property

# textViewForBeginningOfSelection

The text view that contains the first glyph in the selection.

macOS

``` source
unowned(unsafe) var textViewForBeginningOfSelection: NSTextView? { get }
```

## Discussion

This property does not cause layout if the beginning of the selected range is not yet laid out.

## See Also

### Managing the responder chain

func layoutManagerOwnsFirstResponder(in: NSWindow) -> Bool

Indicates whether the first responder in the specified window is a text view for the layout manager.

var firstTextView: NSTextView?

The first text view in the layout manager’s series of text views.

