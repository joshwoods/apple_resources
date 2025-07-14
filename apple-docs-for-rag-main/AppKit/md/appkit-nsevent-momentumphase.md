

- AppKit
- NSEvent
-  momentumPhase 

Instance Property

# momentumPhase

The momentum phase for a scroll or flick gesture.

macOS 10.7+

``` source
var momentumPhase: NSEvent.Phase { get }
```

## Discussion

This property is valid for NSScrollWheel events. With the Magic Mouse and some trackpads, the user can use a scroll wheel or flick gesture resulting in a stream of scroll events that dissipate over time.

The location of these scroll wheel events changes as the user moves the cursor. These events are attached to the view that is under the cursor when the flick occurs. A custom view can use this method to recognize these momentum scroll events and further route the event to the appropriate sub component.

See NSEvent.Phase for possible values.

## See Also

### Getting scroll wheel and flick events

var deltaX: CGFloat

The x-coordinate change for scroll wheel, mouse-move, mouse-drag, and swipe events.

var deltaY: CGFloat

The y-coordinate change for scroll wheel, mouse-move, mouse-drag, and swipe events.

var deltaZ: CGFloat

The z-coordinate change for a scroll wheel, mouse-move, or mouse-drag event.

var hasPreciseScrollingDeltas: Bool

A Boolean value that indicates whether precise scrolling deltas are available.

var scrollingDeltaX: CGFloat

The scroll wheel’s horizontal delta.

var scrollingDeltaY: CGFloat

The scroll wheel’s vertical delta.

var isDirectionInvertedFromDevice: Bool

A Boolean value that indicates whether the user has changed the device inversion.

