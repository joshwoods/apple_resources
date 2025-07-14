

- AppKit
- NSLayoutManager
-  layoutManagerOwnsFirstResponder(in:) 

Instance Method

# layoutManagerOwnsFirstResponder(in:)

Indicates whether the first responder in the specified window is a text view for the layout manager.

macOS

``` source
func layoutManagerOwnsFirstResponder(in window: NSWindow) -> Bool
```

## Parameters 

`window`  

The window whose first responder is tested.

## Return Value

true if the first responder in `window` is a text view associated with the receiver; otherwise, false.

## See Also

### Managing the responder chain

var firstTextView: NSTextView?

The first text view in the layout manager’s series of text views.

var textViewForBeginningOfSelection: NSTextView?

The text view that contains the first glyph in the selection.

