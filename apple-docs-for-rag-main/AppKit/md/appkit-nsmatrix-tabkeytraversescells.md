

- AppKit
- NSMatrix
-  tabKeyTraversesCells 

Instance Property

# tabKeyTraversesCells

A Boolean that indicates whether pressing the Tab key advances the key cell to the next selectable cell.

macOS

``` source
@MainActor
var tabKeyTraversesCells: Bool { get set }
```

## Discussion

When the value of this property is true, pressing the Tab key should advance the key cell to the next selectable cell in the receiver. When the value of this property is false or if there aren’t any selectable cells after the current one, the next view in the window becomes key when the user presses the Tab key.

Pressing Shift-Tab causes the key cell to advance in the opposite direction (if the value of this property is false, or if there aren’t any selectable cells before the current one, the previous view in the window becomes key).

## See Also

### Related Documentation

func selectKeyView(following: NSView)

Gives key view status to the view that follows the given view.

var keyCell: NSCell?

The cell that will be clicked when the user presses the Space bar.

func selectNextKeyView(Any?)

Searches for a candidate next key view and, if it finds one, tries to make it the first responder.

