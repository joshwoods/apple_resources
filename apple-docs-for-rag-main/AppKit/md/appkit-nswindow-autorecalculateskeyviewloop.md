

- AppKit
- NSWindow
-  autorecalculatesKeyViewLoop 

Instance Property

# autorecalculatesKeyViewLoop

A Boolean value that indicates whether the window automatically recalculates the key view loop when views are added.

macOS

``` source
@MainActor
var autorecalculatesKeyViewLoop: Bool { get set }
```

## Discussion

The value of this property is true if the window automatically recalculates the key view loop when views are added; otherwise, false. If autorecalculatesKeyViewLoop is false, the client code must update the key view loop manually or call recalculateKeyViewLoop() to have the window recalculate it.

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

var keyViewSelectionDirection: NSWindow.SelectionDirection

The direction the window is currently using to change the key view.

func recalculateKeyViewLoop()

Marks the key view loop as “dirty” and in need of recalculation.

