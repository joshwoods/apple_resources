

- HIDDriverKit
-  IOHIDPointerEventOptions 

Enumeration

# IOHIDPointerEventOptions

Options that you use to dispatch pointer-related events.

DriverKitmacOS

``` source
typedef enum { ... } IOHIDPointerEventOptions;
```

## Overview

Pass these options to the dispatchRelativePointerEvent or dispatchAbsolutePointerEvent method of IOHIDEventService.

## Topics

### Getting the Pointer Event Option

kIOHIDPointerEventOptionsNoAcceleration

An option for disabling the acceleration logic for this event.

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

dispatchEvent

Dispatches a HID event to the system.

IOHIDKeyboardEventOptions

Options that you use to dispatch keyboard events.

IOHIDScrollEventOptions

Options that you use to dispatch scrolling-related events.

