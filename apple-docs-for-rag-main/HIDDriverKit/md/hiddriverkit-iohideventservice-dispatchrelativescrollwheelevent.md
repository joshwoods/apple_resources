

- HIDDriverKit
- IOHIDEventService
-  dispatchRelativeScrollWheelEvent 

Instance Method

# dispatchRelativeScrollWheelEvent

Dispatches a relative scroll wheel event to the system.

DriverKit 19.0+macOS

``` source
kern_return_t dispatchRelativeScrollWheelEvent(uint64_t timeStamp, IOFixed dx, IOFixed dy, IOFixed dz, IOOptionBits options, bool accelerate);
```

## Parameters 

`timeStamp`  

The timestamp of the event. Use the timestamp of the report element that is the source of the event.

`dx`  

The delta X value.

`dy`  

The delta Y value.

`dz`  

The delta Z value.

`options`  

Additional options for scrolling-related events. Specify `0` for no options. For a list of other values, see IOHIDScrollEventOptions.

`accelerate`  

Scroll events are subject to an acceleration algorithm. Pass in `false` if you don’t wish to have acceleration logic applied to the scroll event.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Call this method from your event service to dispatch a scroll-wheel event to the system. Typically, you call this method when handling a report from the device, after you determine that the report originated from scroll-wheel hardware or otherwise represents a scrolling event.

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

dispatchEvent

Dispatches a HID event to the system.

IOHIDKeyboardEventOptions

Options that you use to dispatch keyboard events.

IOHIDPointerEventOptions

Options that you use to dispatch pointer-related events.

IOHIDScrollEventOptions

Options that you use to dispatch scrolling-related events.

