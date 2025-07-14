

- AppKit
- NSEvent
-  touches(for:) 

Instance Method

# touches(for:)

Returns the touch objects from the event that belong to the specified view.

macOS 10.12+

``` source
func touches(for view: NSView) -> Set
```

## Parameters 

`view`  

The view in which the touches originally occurred.

## Return Value

A set of NSTouch objects that correspond to the touches in the view.

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

func coalescedTouches(for: NSTouch) -> [NSTouch]

Returns all of the touch objects associated with the specified main touch.

class var isMouseCoalescingEnabled: Bool

A Boolean value that indicates whether the system coalesces mouse movement events.

enum GestureAxis

Constants that specify the direction of travel for a gesture.

