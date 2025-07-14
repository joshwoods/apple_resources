

- AppKit
- NSWindow
-  recalculateKeyViewLoop() 

Instance Method

# recalculateKeyViewLoop()

Marks the key view loop as “dirty” and in need of recalculation.

macOS

``` source
@MainActor
func recalculateKeyViewLoop()
```

## Discussion

The key view loop is recalculated the next time someone requests the next or previous key view of the window. The recalculated loop is based on the geometric order of the views in the window.

If you don’t want to maintain the key view loop of your window manually, you can use this method to do it for you. When it’s first loaded, `NSWindow` calls this method automatically if your window doesn’t have a key view loop already established. If you add or remove views later, you can call this method manually to update the window’s key view loop. You can also set the autorecalculatesKeyViewLoop property to have the window recalculate the loop automatically.

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

var autorecalculatesKeyViewLoop: Bool

A Boolean value that indicates whether the window automatically recalculates the key view loop when views are added.

