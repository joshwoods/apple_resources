

- AppKit
- NSEvent
-  allTouches() 

Instance Method

# allTouches()

Returns all touch objects associated with the event.

macOS 10.12+

``` source
func allTouches() -> Set
```

## Return Value

A set of NSTouch objects that correspond to the touches of this event.

## Discussion

If the touches originate in different views or windows, each NSTouch object may have a different responder object.

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

func touches(for: NSView) -> Set&lt;NSTouch>

Returns the touch objects from the event that belong to the specified view.

func coalescedTouches(for: NSTouch) -> [NSTouch]

Returns all of the touch objects associated with the specified main touch.

class var isMouseCoalescingEnabled: Bool

A Boolean value that indicates whether the system coalesces mouse movement events.

enum GestureAxis

Constants that specify the direction of travel for a gesture.

