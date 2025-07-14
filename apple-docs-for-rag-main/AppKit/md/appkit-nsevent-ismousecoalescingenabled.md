

- AppKit
- NSEvent
-  isMouseCoalescingEnabled 

Type Property

# isMouseCoalescingEnabled

A Boolean value that indicates whether the system coalesces mouse movement events.

macOS 10.5+

``` source
class var isMouseCoalescingEnabled: Bool { get set }
```

## Discussion

Mouse movement events include mouse-moved, mouse-dragged, and tablet events. If this property is true, coalescing is enabled; otherwise, it’s disabled. The default value of this property is true.

## See Also

### Getting gesture and touch information

var phase: NSEvent.Phase

The phase of a gesture event, such as a magnify, scroll, or pressure change.

struct Phase

Constants that represent the possible phases during an event phase.

var magnification: CGFloat

The amount of change to add to a magnification gesture.

func touches(matching: NSTouch.Phase, in: NSView?) -> Set&lt;NSTouch>

Returns the touch objects associated with the specified phase.

func allTouches() -> Set&lt;NSTouch>

Returns all touch objects associated with the event.

func touches(for: NSView) -> Set&lt;NSTouch>

Returns the touch objects from the event that belong to the specified view.

func coalescedTouches(for: NSTouch) -> [NSTouch]

Returns all of the touch objects associated with the specified main touch.

enum GestureAxis

Constants that specify the direction of travel for a gesture.

