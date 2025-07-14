

- AppKit
- NSView
-  previousKeyView 

Instance Property

# previousKeyView

The view object preceding the current view in the key view loop.

macOS

``` source
@MainActor
unowned(unsafe) var previousKeyView: NSView? { get }
```

## Discussion

The value in this property is `nil` if there is no view preceding the current view in the key view loop. The view in this property should, if possible, be made first responder when the user navigates backward from the current view using keyboard interface control.

## See Also

### Related Documentation

func selectKeyView(following: NSView)

Gives key view status to the view that follows the given view.

func selectNextKeyView(Any?)

Searches for a candidate next key view and, if it finds one, tries to make it the first responder.

func selectPreviousKeyView(Any?)

Searches for a candidate previous key view and, if it finds one, tries to make it the first responder.

func selectKeyView(preceding: NSView)

Gives key view status to the view that precedes the given view.

### Managing the Key-View Loop

var canBecomeKeyView: Bool

A Boolean value indicating whether the view can become key view.

var needsPanelToBecomeKey: Bool

A Boolean value indicating whether the view needs its panel to become the key window before it can handle keyboard input and navigation.

var nextKeyView: NSView?

The view object that follows the current view in the key view loop.

var nextValidKeyView: NSView?

The closest view object in the key view loop that follows the current view in the key view loop and accepts first responder status.

var previousValidKeyView: NSView?

The closest view object in the key view loop that precedes the current view and accepts first responder status.

