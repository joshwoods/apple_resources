

- UIKit
- UIControl
-  isTracking 

Instance Property

# isTracking

A Boolean value that indicates whether the control is currently tracking touch events.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isTracking: Bool { get }
```

## Discussion

While tracking of a touch event is in progress, the control sets the value of this property to true. When tracking ends or is canceled for any reason, it sets this property to false.

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

var isTouchInside: Bool

A Boolean value that indicates whether a tracked touch event is currently inside the control’s bounds.

