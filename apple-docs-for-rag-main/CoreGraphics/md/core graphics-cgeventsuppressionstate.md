

- Core Graphics
-  CGEventSuppressionState 

Enumeration

# CGEventSuppressionState

Specify the event suppression states that can occur after posting an event.

Mac CatalystmacOS

``` source
enum CGEventSuppressionState
```

## Overview

These constants specify the types of event suppression intervals during which an event filter is applied after posting an event.

## Topics

### Constants

case eventSuppressionStateSuppressionInterval

Specifies that certain local hardware events may be suppressed for a short interval after posting an event.

case eventSuppressionStateRemoteMouseDrag

Specifies that certain local hardware events may be suppressed during a mouse drag operation (mouse movement with the left or only mouse button down).

case numberOfEventSuppressionStates

### Enumeration Cases

case numberOfEventSuppressionStates

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

enum CGEventField

Constants used as keys to access specialized fields in low-level events.

struct CGEventFilterMask

Specify masks for classes of low-level events that can be filtered during event suppression states.

struct CGEventFlags

Constants that indicate the modifier key state at the time an event is created, as well as other event-related states.

enum CGEventMouseSubtype

Constants used with the CGEventField.mouseEventSubtype event field.

enum CGEventSourceStateID

Constants that specify the possible source states of an event source.

enum CGEventTapLocation

Constants that specify possible tapping points for events.

enum CGEventTapOptions

Constants that specify whether a new event tap is an active filter or a passive listener.

