

- UIKit
- UIControl
-  cancelTracking(with:) 

Instance Method

# cancelTracking(with:)

Notifies the control to cancel tracking related to the specified event.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func cancelTracking(with event: UIEvent?)
```

## Parameters 

`event`  

An event object related to touches that occurred in the control. This parameter might be `nil`, indicating that the cancelation was caused by something other than an event, such as the view being removed from the window.

## Discussion

The control calls this method when a control-related touch event is canceled. The default implementation cancels any ongoing tracking and updates the control’s state information. Subclasses can override this method and use it to perform any actions relevant to the cancellation of the touch sequence. You should also use it to perform any cleanup associated with tracking the event.

If you override this method, you must call `super` at some point in your implementation.

## See Also

### Tracking touches and redrawing controls

func beginTracking(UITouch, with: UIEvent?) -> Bool

Notifies the control when a touch event enters the control’s bounds.

func continueTracking(UITouch, with: UIEvent?) -> Bool

Notifies the control when a touch event for the control updates.

func endTracking(UITouch?, with: UIEvent?)

Notifies the control when a touch event associated with the control ends.

var isTracking: Bool

A Boolean value that indicates whether the control is currently tracking touch events.

var isTouchInside: Bool

A Boolean value that indicates whether a tracked touch event is currently inside the control’s bounds.

