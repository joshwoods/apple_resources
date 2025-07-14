

- AppKit
- NSWindow
-  selectPreviousKeyView(\_:) 

Instance Method

# selectPreviousKeyView(\_:)

Searches for a candidate previous key view and, if it finds one, tries to make it the first responder.

macOS

``` source
@MainActor
func selectPreviousKeyView(_ sender: Any?)
```

## Parameters 

`sender`  

The message’s sender.

## Discussion

The candidate is one of the following (which this function searches for in this order):

- The current first responder’s previous valid key view, which the previousValidKeyView method of `NSView` returns

- The initialFirstResponder designates as the window’s initial first responder if it returns true to an acceptsFirstResponder message

- Otherwise, the initial first responder’s previous valid key view, which may be `nil`

## See Also

### Managing the Key View Loop

func selectKeyView(preceding: NSView)

Gives key view status to the view that precedes the given view.

func selectKeyView(following: NSView)

Gives key view status to the view that follows the given view.

func selectNextKeyView(Any?)

Searches for a candidate next key view and, if it finds one, tries to make it the first responder.

var keyViewSelectionDirection: NSWindow.SelectionDirection

The direction the window is currently using to change the key view.

var autorecalculatesKeyViewLoop: Bool

A Boolean value that indicates whether the window automatically recalculates the key view loop when views are added.

func recalculateKeyViewLoop()

Marks the key view loop as “dirty” and in need of recalculation.

