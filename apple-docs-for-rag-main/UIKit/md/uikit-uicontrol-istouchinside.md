

- UIKit
- UIControl
-  isTouchInside 

Instance Property

# isTouchInside

A Boolean value that indicates whether a tracked touch event is currently inside the control’s bounds.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isTouchInside: Bool { get }
```

## Return Value

true if the location of the most recent touch event is inside the control’s bounds or false if it is not.

## Discussion

While tracking of a touch event is ongoing, the control updates the value of this property to indicate whether the most recent touch is still inside the control’s bounds. The control uses this information to trigger specific events. For example, touch events entering or exiting a control trigger appropriate drag events.

## See Also

### Tracking touches and redrawing controls

func beginTracking(UITouch, with: UIEvent?) -> Bool

Notifies the control when a touch event enters the control’s bounds.

func continueTracking(UITouch, with: UIEvent?) -> Bool

Notifies the control when a touch event for the control updates.

func endTracking(UITouch?, with: UIEvent?)

Notifies the control when a touch event associated with the control ends.

func cancelTracking(with: UIEvent?)

Notifies the control to cancel tracking related to the specified event.

var isTracking: Bool

A Boolean value that indicates whether the control is currently tracking touch events.

