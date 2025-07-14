

- AppKit
- NSWindow
-  delegate 

Instance Property

# delegate

The window’s delegate.

macOS

``` source
@MainActor
weak var delegate: (any NSWindowDelegate)? { get set }
```

## Discussion

The value of this property is `nil` if the window doesn’t have a delegate.

A window object’s delegate is inserted in the responder chain after the window itself and is informed of various actions by the window through delegation messages.

## See Also

### Related Documentation

func tryToPerform(Selector, with: Any?) -> Bool

Dispatches action messages with a given argument.

func sendAction(Selector, to: Any?, from: Any?) -> Bool

Sends the given action message to the given target.

### Managing the Window’s Behavior

protocol NSWindowDelegate

A set of optional methods that a window’s delegate can implement to respond to events, such as window resizing, moving, exposing, and minimizing.

