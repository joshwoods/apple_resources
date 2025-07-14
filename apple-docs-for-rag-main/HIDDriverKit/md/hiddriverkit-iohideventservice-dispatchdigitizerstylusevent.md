

- HIDDriverKit
- IOHIDEventService
-  dispatchDigitizerStylusEvent 

Instance Method

# dispatchDigitizerStylusEvent

Dispatches a digitizer stylus event to the system.

DriverKit 19.0+macOS

``` source
kern_return_t dispatchDigitizerStylusEvent(uint64_t timeStamp, IOHIDDigitizerStylusData * stylusData);
```

## Parameters 

`timeStamp`  

The timestamp of the event. Use the timestamp of the report element that is the source of the event.

`stylusData`  

A structure containing the stylus data. For more information, see IOHIDDigitizerStylusData.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

The default implementation of this method does nothing. Subclasses must override it to dispatch stylus events.

## See Also

### Dispatching Events

dispatchKeyboardEvent

Dispatches a keyboard-related event to the system.

dispatchRelativePointerEvent

Dispatches a relative pointer event to the system.

dispatchAbsolutePointerEvent

Dispatches an absolute pointer event to the system.

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

