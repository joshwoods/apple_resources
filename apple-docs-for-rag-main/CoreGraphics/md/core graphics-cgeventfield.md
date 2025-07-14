

- Core Graphics
-  CGEventField 

Enumeration

# CGEventField

Constants used as keys to access specialized fields in low-level events.

Mac CatalystmacOS

``` source
enum CGEventField
```

## Overview

These constants are used as keys to access certain specialized event fields when using low-level accessor functions such as getIntegerValueField(_:), setIntegerValueField(_:value:), getDoubleValueField(_:), and setDoubleValueField(_:value:).

## Topics

### Constants

case mouseEventNumber

Key to access an integer field that contains the mouse button event number. Matching mouse-down and mouse-up events will have the same event number.

case mouseEventClickState

Key to access an integer field that contains the mouse button click state. A click state of 1 represents a single click. A click state of 2 represents a double-click. A click state of 3 represents a triple-click.

case mouseEventPressure

Key to access a double field that contains the mouse button pressure. The pressure value may range from 0 to 1, with 0 representing the mouse being up. This value is commonly set by tablet pens mimicking a mouse.

case mouseEventButtonNumber

Key to access an integer field that contains the mouse button number. For information about the possible values, see CGMouseButton.

case mouseEventDeltaX

Key to access an integer field that contains the horizontal mouse delta since the last mouse movement event.

case mouseEventDeltaY

Key to access an integer field that contains the vertical mouse delta since the last mouse movement event.

case mouseEventInstantMouser

Key to access an integer field. The value is non-zero if the event should be ignored by the Inkwell subsystem.

case mouseEventSubtype

Key to access an integer field that encodes the mouse event subtype as a `kCFNumberIntType`.

case keyboardEventAutorepeat

Key to access an integer field, non-zero when this is an autorepeat of a key-down, and zero otherwise.

case keyboardEventKeycode

Key to access an integer field that contains the virtual keycode of the key-down or key-up event.

case keyboardEventKeyboardType

Key to access an integer field that contains the keyboard type identifier.

case scrollWheelEventDeltaAxis1

Key to access an integer field that contains scrolling data. This field typically contains the change in vertical position since the last scrolling event from a Mighty Mouse scroller or a single-wheel mouse scroller.

case scrollWheelEventDeltaAxis2

Key to access an integer field that contains scrolling data. This field typically contains the change in horizontal position since the last scrolling event from a Mighty Mouse scroller.

case scrollWheelEventDeltaAxis3

This field is not used.

case scrollWheelEventFixedPtDeltaAxis1

Key to access a field that contains scrolling data. The scrolling data represents a line-based or pixel-based change in vertical position since the last scrolling event from a Mighty Mouse scroller or a single-wheel mouse scroller. The scrolling data uses a fixed-point 16.16 signed integer format. For example, if the field contains a value of 1.0, the integer 0x00010000 is returned by `CGEventGetIntegerValueField`. If this key is passed to `CGEventGetDoubleValueField`, the fixed-point value is converted to a double value.

case scrollWheelEventFixedPtDeltaAxis2

Key to access a field that contains scrolling data. The scrolling data represents a line-based or pixel-based change in horizontal position since the last scrolling event from a Mighty Mouse scroller. The scrolling data uses a fixed-point 16.16 signed integer format. For example, if the field contains a value of 1.0, the integer 0x00010000 is returned by `CGEventGetIntegerValueField`. If this key is passed to `CGEventGetDoubleValueField`, the fixed-point value is converted to a double value.

case scrollWheelEventFixedPtDeltaAxis3

This field is not used.

case scrollWheelEventPointDeltaAxis1

Key to access an integer field that contains pixel-based scrolling data. The scrolling data represents the change in vertical position since the last scrolling event from a Mighty Mouse scroller or a single-wheel mouse scroller.

case scrollWheelEventPointDeltaAxis2

Key to access an integer field that contains pixel-based scrolling data. The scrolling data represents the change in horizontal position since the last scrolling event from a Mighty Mouse scroller.

case scrollWheelEventPointDeltaAxis3

This field is not used.

case scrollWheelEventInstantMouser

Key to access an integer field that indicates whether the event should be ignored by the Inkwell subsystem. If the value is non-zero, the event should be ignored.

case tabletEventPointX

Key to access an integer field that contains the absolute X coordinate in tablet space at full tablet resolution.

case tabletEventPointY

Key to access an integer field that contains the absolute Y coordinate in tablet space at full tablet resolution.

case tabletEventPointZ

Key to access an integer field that contains the absolute Z coordinate in tablet space at full tablet resolution.

case tabletEventPointButtons

Key to access an integer field that contains the tablet button state. Bit 0 is the first button, and a set bit represents a closed or pressed button. Up to 16 buttons are supported.

case tabletEventPointPressure

Key to access a double field that contains the tablet pen pressure. A value of 0.0 represents no pressure, and 1.0 represents maximum pressure.

case tabletEventTiltX

Key to access a double field that contains the horizontal tablet pen tilt. A value of 0.0 represents no tilt, and 1.0 represents maximum tilt.

case tabletEventTiltY

Key to access a double field that contains the vertical tablet pen tilt. A value of 0.0 represents no tilt, and 1.0 represents maximum tilt.

case tabletEventRotation

Key to access a double field that contains the tablet pen rotation.

case tabletEventTangentialPressure

Key to access a double field that contains the tangential pressure on the device. A value of 0.0 represents no pressure, and 1.0 represents maximum pressure.

case tabletEventDeviceID

Key to access an integer field that contains the system-assigned unique device ID.

case tabletEventVendor1

Key to access an integer field that contains a vendor-specified value.

case tabletEventVendor2

Key to access an integer field that contains a vendor-specified value.

case tabletEventVendor3

Key to access an integer field that contains a vendor-specified value.

case tabletProximityEventVendorID

Key to access an integer field that contains the vendor-defined ID, typically the USB vendor ID.

case tabletProximityEventTabletID

Key to access an integer field that contains the vendor-defined tablet ID, typically the USB product ID.

case tabletProximityEventPointerID

Key to access an integer field that contains the vendor-defined ID of the pointing device.

case tabletProximityEventDeviceID

Key to access an integer field that contains the system-assigned device ID.

case tabletProximityEventSystemTabletID

Key to access an integer field that contains the system-assigned unique tablet ID.

case tabletProximityEventVendorPointerType

Key to access an integer field that contains the vendor-assigned pointer type.

case tabletProximityEventVendorPointerSerialNumber

Key to access an integer field that contains the vendor-defined pointer serial number.

case tabletProximityEventVendorUniqueID

Key to access an integer field that contains the vendor-defined unique ID.

case tabletProximityEventCapabilityMask

Key to access an integer field that contains the device capabilities mask.

case tabletProximityEventPointerType

Key to access an integer field that contains the pointer type.

case tabletProximityEventEnterProximity

Key to access an integer field that indicates whether the pen is in proximity to the tablet. The value is non-zero if the pen is in proximity to the tablet and zero when leaving the tablet.

case eventTargetProcessSerialNumber

Key to access a field that contains the event target process serial number. The value is a 64-bit long word.

case eventTargetUnixProcessID

Key to access a field that contains the event target Unix process ID.

case eventSourceUnixProcessID

Key to access a field that contains the event source Unix process ID.

case eventSourceUserData

Key to access a field that contains the event source user-supplied data, up to 64 bits.

case eventSourceUserID

Key to access a field that contains the event source Unix effective UID.

case eventSourceGroupID

Key to access a field that contains the event source Unix effective GID.

case eventSourceStateID

Key to access a field that contains the event source state ID used to create this event.

case scrollWheelEventIsContinuous

Key to access an integer field that indicates whether a scrolling event contains continuous, pixel-based scrolling data. The value is non-zero when the scrolling data is pixel-based and zero when the scrolling data is line-based.

case mouseEventWindowUnderMousePointer

case mouseEventWindowUnderMousePointerThatCanHandleThisEvent

case scrollWheelEventMomentumPhase

case scrollWheelEventScrollCount

case scrollWheelEventScrollPhase

### Enumeration Cases

case mouseEventWindowUnderMousePointer

case mouseEventWindowUnderMousePointerThatCanHandleThisEvent

case scrollWheelEventMomentumPhase

case scrollWheelEventScrollCount

case scrollWheelEventScrollPhase

case eventUnacceleratedPointerMovementX

case eventUnacceleratedPointerMovementY

case scrollWheelEventAcceleratedDeltaAxis1

case scrollWheelEventAcceleratedDeltaAxis2

case scrollWheelEventMomentumOptionPhase

case scrollWheelEventRawDeltaAxis1

case scrollWheelEventRawDeltaAxis2

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

struct CGCaptureOptions

Configuration parameters that are used when capturing displays.

enum CGColorConversionInfoTransformType

Constants describing how a color conversion uses color spaces.

enum CGColorRenderingIntent

Handling options for colors that are not located within the destination color space of a graphics context.

struct CGConfigureOption

The scope of the changes in a display configuration transaction.

struct CGDisplayChangeSummaryFlags

The configuration parameters that are passed to a display reconfiguration callback function.

enum CGDisplayStreamFrameStatus

Describes a frame update event.

enum CGDisplayStreamUpdateRectType

Use these constants to determine which rectangles your app is interested in.

enum CGError

A uniform type for result codes returned by functions in Core Graphics.

struct CGEventFilterMask

Specify masks for classes of low-level events that can be filtered during event suppression states.

struct CGEventFlags

Constants that indicate the modifier key state at the time an event is created, as well as other event-related states.

enum CGEventMouseSubtype

Constants used with the CGEventField.mouseEventSubtype event field.

enum CGEventSourceStateID

Constants that specify the possible source states of an event source.

enum CGEventSuppressionState

Specify the event suppression states that can occur after posting an event.

enum CGEventTapLocation

Constants that specify possible tapping points for events.

enum CGEventTapOptions

Constants that specify whether a new event tap is an active filter or a passive listener.

