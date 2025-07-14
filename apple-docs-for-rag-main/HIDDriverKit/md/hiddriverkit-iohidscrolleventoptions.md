

- HIDDriverKit
-  IOHIDScrollEventOptions 

Enumeration

# IOHIDScrollEventOptions

Options that you use to dispatch scrolling-related events.

DriverKitmacOS

``` source
typedef enum { ... } IOHIDScrollEventOptions;
```

## Overview

Pass these options to the dispatchRelativeScrollWheelEvent method of IOHIDEventService.

## Topics

### Getting the Scroll Event Option

kIOHIDScrollEventOptionsNoAcceleration

An option for not applying the default acceleration algorithm to this event.

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

IOHIDPointerEventOptions

Options that you use to dispatch pointer-related events.

