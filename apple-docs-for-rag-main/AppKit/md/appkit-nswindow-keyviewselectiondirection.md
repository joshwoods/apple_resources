

- AppKit
- NSWindow
-  keyViewSelectionDirection 

Instance Property

# keyViewSelectionDirection

The direction the window is currently using to change the key view.

macOS

``` source
@MainActor
var keyViewSelectionDirection: NSWindow.SelectionDirection { get }
```

## Discussion

The value of this property can be one of the values described in NSWindow.SelectionDirection.

## See Also

### Managing the Key View Loop

func selectKeyView(preceding: NSView)

Gives key view status to the view that precedes the given view.

func selectKeyView(following: NSView)

Gives key view status to the view that follows the given view.

func selectPreviousKeyView(Any?)

Searches for a candidate previous key view and, if it finds one, tries to make it the first responder.

func selectNextKeyView(Any?)

Searches for a candidate next key view and, if it finds one, tries to make it the first responder.

var autorecalculatesKeyViewLoop: Bool

A Boolean value that indicates whether the window automatically recalculates the key view loop when views are added.

func recalculateKeyViewLoop()

Marks the key view loop as “dirty” and in need of recalculation.

