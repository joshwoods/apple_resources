

- AppKit
- NSEvent
-  magnification 

Instance Property

# magnification

The amount of change to add to a magnification gesture.

macOS 10.5+

``` source
var magnification: CGFloat { get }
```

## Discussion

The change in magnification that should be added to the current scaling of an item to achieve the new scale factor. This message is valid only for events of type NSEvent.EventType.magnify.

## See Also

### Getting gesture and touch information

var phase: NSEvent.Phase

The phase of a gesture event, such as a magnify, scroll, or pressure change.

struct Phase

Constants that represent the possible phases during an event phase.

func touches(matching: NSTouch.Phase, in: NSView?) -> Set&lt;NSTouch>

Returns the touch objects associated with the specified phase.

func allTouches() -> Set&lt;NSTouch>

Returns all touch objects associated with the event.

func touches(for: NSView) -> Set&lt;NSTouch>

Returns the touch objects from the event that belong to the specified view.

func coalescedTouches(for: NSTouch) -> [NSTouch]

Returns all of the touch objects associated with the specified main touch.

class var isMouseCoalescingEnabled: Bool

A Boolean value that indicates whether the system coalesces mouse movement events.

enum GestureAxis

Constants that specify the direction of travel for a gesture.

