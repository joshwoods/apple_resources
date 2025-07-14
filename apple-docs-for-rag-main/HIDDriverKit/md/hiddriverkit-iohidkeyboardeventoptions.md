

- HIDDriverKit
-  IOHIDKeyboardEventOptions 

Enumeration

# IOHIDKeyboardEventOptions

Options that you use to dispatch keyboard events.

DriverKitmacOS

``` source
typedef enum { ... } IOHIDKeyboardEventOptions;
```

## Overview

Pass these options to the dispatchKeyboardEvent method of IOHIDEventService.

## Topics

### Getting the Keyboard Event Option

kIOHIDKeyboardEventOptionsNoKeyRepeat

An option for not applying the default key repeat logic to the event.

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

IOHIDPointerEventOptions

Options that you use to dispatch pointer-related events.

IOHIDScrollEventOptions

Options that you use to dispatch scrolling-related events.

