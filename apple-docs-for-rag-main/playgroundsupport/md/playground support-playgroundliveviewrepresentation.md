

- Playground Support
-  PlaygroundLiveViewRepresentation 

Enumeration

# PlaygroundLiveViewRepresentation

The supported types for displaying for live views in playgrounds.

macOS 11.0+Xcode 10.2+Swift Playgrounds 2.0+

``` source
enum PlaygroundLiveViewRepresentation
```

## Topics

### Displaying UIKit Views

case view(UIView)

A UIKit view that's displayed as the live view.

case viewController(UIViewController)

A UIKit view controller whose view is displayed as the live view.

### Displaying AppKit Views

case view(NSView)

An AppKit view that's displayed as the live view.

case viewController(NSViewController)

An AppKit view controller whose view is displayed as the live view.

## See Also

### Live Views

protocol PlaygroundLiveViewable

A protocol that displays an instance as a live view in a playground.

protocol PlaygroundLiveViewSafeAreaContainer

A protocol that ensures that views fit without obstruction within the Swift Playgrounds user interface.

