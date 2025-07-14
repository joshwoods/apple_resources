

- UIKit
- UIControl
-  endTracking(\_:with:) 

Instance Method

# endTracking(\_:with:)

Notifies the control when a touch event associated with the control ends.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func endTracking(
    _ touch: UITouch?,
    with event: UIEvent?
)
```

## Parameters 

`touch`  

The touch object containing the final touch information.

`event`  

The event object containing the touch event.

## Discussion

This method is called at the end of a sequence of touch events inside the control’s bounds. Subclasses can override this method and use it to perform any actions relevant to the completion of the touch sequence. You should also use it to perform any cleanup associated with tracking the event.

If you override this method, you must call `super` at some point in your implementation. The default implementation updates the isTracking property of the control.

## See Also

### Tracking touches and redrawing controls

func beginTracking(UITouch, with: UIEvent?) -> Bool

Notifies the control when a touch event enters the control’s bounds.

func continueTracking(UITouch, with: UIEvent?) -> Bool

Notifies the control when a touch event for the control updates.

func cancelTracking(with: UIEvent?)

Notifies the control to cancel tracking related to the specified event.

var isTracking: Bool

A Boolean value that indicates whether the control is currently tracking touch events.

var isTouchInside: Bool

A Boolean value that indicates whether a tracked touch event is currently inside the control’s bounds.

