

- AppKit
- NSWindow
-  selectKeyView(following:) 

Instance Method

# selectKeyView(following:)

Gives key view status to the view that follows the given view.

macOS

``` source
@MainActor
func selectKeyView(following view: NSView)
```

## Parameters 

`view`  

The view whose following view in the key view loop to seek.

## Discussion

Sends the nextValidKeyView message to `view` and, if that message returns an `NSView` object, invokes makeFirstResponder(_:) with the returned object.

## See Also

### Managing the Key View Loop

func selectKeyView(preceding: NSView)

Gives key view status to the view that precedes the given view.

func selectPreviousKeyView(Any?)

Searches for a candidate previous key view and, if it finds one, tries to make it the first responder.

func selectNextKeyView(Any?)

Searches for a candidate next key view and, if it finds one, tries to make it the first responder.

var keyViewSelectionDirection: NSWindow.SelectionDirection

The direction the window is currently using to change the key view.

var autorecalculatesKeyViewLoop: Bool

A Boolean value that indicates whether the window automatically recalculates the key view loop when views are added.

func recalculateKeyViewLoop()

Marks the key view loop as “dirty” and in need of recalculation.

