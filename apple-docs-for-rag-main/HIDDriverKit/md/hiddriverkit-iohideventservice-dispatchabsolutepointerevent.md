

- HIDDriverKit
- IOHIDEventService
-  dispatchAbsolutePointerEvent 

Instance Method

# dispatchAbsolutePointerEvent

Dispatches an absolute pointer event to the system.

DriverKit 19.0+macOS

``` source
kern_return_t dispatchAbsolutePointerEvent(uint64_t timeStamp, IOFixed x, IOFixed y, uint32_t buttonState, IOOptionBits options, bool accelerate);
```

## Parameters 

`timeStamp`  

The timestamp of the event. Use the timestamp of the report element that is the source of the event.

`x`  

The X value, specified in the range `0` to `1`.

`y`  

The Y value, specified in the range `0` to `1`.

`buttonState`  

The current button state, if any.

`options`  

Additional options for pointer events. Specify `0` for no options. For a list of other values, see IOHIDPointerEventOptions.

`accelerate`  

A Boolean value indicating whether to apply the acceleration algorithm to the pointer event. Specify `false` if you don’t want to apply that logic.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Call this method from your event service to dispatch a keyboard event to the system. Typically, you call this method after determining that a report contains data representing a mouse- or pointer-related event.

## See Also

### Dispatching Events

dispatchKeyboardEvent

Dispatches a keyboard-related event to the system.

dispatchRelativePointerEvent

Dispatches a relative pointer event to the system.

dispatchDigitizerStylusEvent

Dispatches a digitizer stylus event to the system.

dispatchDigitizerTouchEvent

Dispatches a digitizer touch event to the system.

dispatchRelativeScrollWheelEvent

Dispatches a relative scroll wheel event to the system.

dispatchEvent

Dispatches a HID event to the system.

IOHIDKeyboardEventOptions

Options that you use to dispatch keyboard events.

IOHIDPointerEventOptions

Options that you use to dispatch pointer-related events.

IOHIDScrollEventOptions

Options that you use to dispatch scrolling-related events.

