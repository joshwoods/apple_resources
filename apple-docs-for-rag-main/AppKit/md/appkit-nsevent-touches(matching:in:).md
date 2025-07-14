

- AppKit
- NSEvent
-  touches(matching:in:) 

Instance Method

# touches(matching:in:)

Returns the touch objects associated with the specified phase.

macOS 10.6+

``` source
func touches(
    matching phase: NSTouch.Phase,
    in view: NSView?
) -> Set
```

## Parameters 

`phase`  

The touch phase for which you want touches.

`view`  

The view for which touches are wanted. Touches that target this view, or any of the view’s descendants will be returned. Passing `nil` as the view gets all touches regardless of their targeted view.

## Return Value

A set of applicable NSTouch objects.

## Discussion

This method is only valid for gesture events (gesture, magnify, swipe, rotate, etc.).

## See Also

### Getting gesture and touch information

var phase: NSEvent.Phase

The phase of a gesture event, such as a magnify, scroll, or pressure change.

struct Phase

Constants that represent the possible phases during an event phase.

var magnification: CGFloat

The amount of change to add to a magnification gesture.

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

