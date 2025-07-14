

- AppKit
- NSEvent
-  phase 

Instance Property

# phase

The phase of a gesture event, such as a magnify, scroll, or pressure change.

macOS 10.7+

``` source
var phase: NSEvent.Phase { get }
```

## Discussion

A gesture phase corresponds to a fluid gesture event. As a gesture event occurs, its phase begins with began and ends with either ended or cancelled. All the gesture events are sent to the view under the cursor when the began occurred.

Technically, a gesture scroll event starts with a began phase and ends with a ended. However, when the user puts two fingers down on a trackpad, the trackpad issues mayBegin, followed by began, cancelled, or ended. The mayBegin event phase signals that scrolling is about to begin before the gesture has technically started. A Magic Mouse does not issue mayBegin scroll wheel events.

A pressure event (type NSEvent.EventType.pressure) is a fluid gesture. Like the other fluid gesture events, it has a phase that describes the sequence of the pressure gesture stream.

Legacy scroll wheel events (say from a Mighty Mouse) and momentum scroll wheel events both have a phase of NSEventPhaseNone. (Legacy scroll wheel events also have a momentumPhase of NSEventPhaseNone.) To learn more about scroll wheel events, see Handling Trackpad Events.

See NSEvent.Phase for possible values.

## See Also

### Getting gesture and touch information

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

class var isMouseCoalescingEnabled: Bool

A Boolean value that indicates whether the system coalesces mouse movement events.

enum GestureAxis

Constants that specify the direction of travel for a gesture.

