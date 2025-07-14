

- HIDDriverKit
- IOHIDEventService
-  dispatchKeyboardEvent 

Instance Method

# dispatchKeyboardEvent

Dispatches a keyboard-related event to the system.

DriverKit 19.0+macOS

``` source
kern_return_t dispatchKeyboardEvent(uint64_t timeStamp, uint32_t usagePage, uint32_t usage, uint32_t value, IOOptionBits options, bool repeat);
```

## Parameters 

`timeStamp`  

The timestamp of the event. Use the timestamp of the report element that is the source of the event.

`usagePage`  

The HID usage page to associate with the event. For a list of possible values, see Usage Pages.

`usage`  

The HID usage code indicating the specific type of the event. For a list of possible usage values, see HID Usage Tables.

`value`  

The value associated with the event.

`options`  

Additional options for keyboard events. Specify `0` for no options. For a list of other values, see IOHIDKeyboardEventOptions.

`repeat`  

The autorepeat behavior to apply when the user holds down a key. Specify `true` to apply the default behavior, which repeats the key event after a user-configurable amount of time elapses. Specify `false` to prevent the delivery of repeat events.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Call this method from your event service to dispatch a keyboard event to the system. Typically, you call this method when handling a report from the device, after you determine that the report contains a keyboard-related event.

## See Also

### Dispatching Events

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

dispatchEvent

Dispatches a HID event to the system.

IOHIDKeyboardEventOptions

Options that you use to dispatch keyboard events.

IOHIDPointerEventOptions

Options that you use to dispatch pointer-related events.

IOHIDScrollEventOptions

Options that you use to dispatch scrolling-related events.

