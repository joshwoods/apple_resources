

- HIDDriverKit
- IOHIDEventService
-  dispatchEvent 

Instance Method

# dispatchEvent

Dispatches a HID event to the system.

DriverKit 19.0+macOS

``` source
void dispatchEvent(IOHIDEvent * event);
```

## Parameters 

`event`  

The event to dispatch.

## Discussion

This method is a funnel point for dispatching events to the system’s registered clients. You can also call it directly to dispatch events for which you create an `IOHIDEvent` object.

## See Also

### Dispatching Events

dispatchKeyboardEvent

Dispatches a keyboard-related event to the system.

dispatchRelativePointerEvent

Dispatches a relative pointer event to the system.

dispatchAbsolutePointerEvent

Dispatches an absolute pointer event to the system.

dispatchDigitizerStylusEvent

Dispatches a digitizer stylus event to the system.

dispatchDigitizerTouchEvent

Dispatches a digitizer touch event to the system.

dispatchRelativeScrollWheelEvent

Dispatches a relative scroll wheel event to the system.

IOHIDKeyboardEventOptions

Options that you use to dispatch keyboard events.

IOHIDPointerEventOptions

Options that you use to dispatch pointer-related events.

IOHIDScrollEventOptions

Options that you use to dispatch scrolling-related events.

