

- AppKit
- NSView
-  nextKeyView 

Instance Property

# nextKeyView

The view object that follows the current view in the key view loop.

macOS

``` source
@MainActor
unowned(unsafe) var nextKeyView: NSView? { get set }
```

## Discussion

The value in this property is `nil` if there is no next view in the key view loop. You can assign a view to this property to make that view the next view in the loop. The view in this property should, if possible, be made first responder when the user navigates forward from the view using keyboard interface control.

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

var nextValidKeyView: NSView?

The closest view object in the key view loop that follows the current view in the key view loop and accepts first responder status.

var previousKeyView: NSView?

The view object preceding the current view in the key view loop.

var previousValidKeyView: NSView?

The closest view object in the key view loop that precedes the current view and accepts first responder status.

