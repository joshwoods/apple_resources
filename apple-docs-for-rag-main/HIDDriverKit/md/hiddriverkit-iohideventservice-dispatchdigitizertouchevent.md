

- HIDDriverKit
- IOHIDEventService
-  dispatchDigitizerTouchEvent 

Instance Method

# dispatchDigitizerTouchEvent

Dispatches a digitizer touch event to the system.

DriverKit 19.0+macOS

``` source
kern_return_t dispatchDigitizerTouchEvent(uint64_t timeStamp, IOHIDDigitizerTouchData * touchData, uint32_t touchDataCount);
```

## Parameters 

`timeStamp`  

The timestamp of the event. Use the timestamp of the report element that is the source of the event.

`touchData`  

An array of structures containing the data for the individual touches. For more information, see IOHIDDigitizerTouchData.

`touchDataCount`  

The number of structures in the `touchData` parameter.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

The default implementation of this method does nothing. Subclasses must override it to dispatch touch events.

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

