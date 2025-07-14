

- AppKit
- NSView
-  wantsRestingTouches 

Instance Property

# wantsRestingTouches

A Boolean value indicating whether the view wants resting touches.

macOS 10.6+

``` source
@MainActor
var wantsRestingTouches: Bool { get set }
```

## Discussion

A resting touch occurs when a user rests their thumb on a device (for example, the glass trackpad of a MacBook). By default, these touches are not delivered and are not included in the event’s set of touches. Touches may transition in and out of resting at any time. Unless the view wants resting touches, began / ended events are simulated as touches transition from resting to active and vice versa.

The default value of this property is false, which indicates that the view does not want resting touches.

## See Also

### Handling Touch Events

var allowedTouchTypes: NSTouch.TouchTypeMask

The types of touch interactions the view allows.

var candidateListTouchBarItem: NSCandidateListTouchBarItem&lt;AnyObject>?

