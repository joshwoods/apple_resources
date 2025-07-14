

- Core Graphics
-  CGEventType 

Enumeration

# CGEventType

Constants that specify the different types of input events.

Mac CatalystmacOS

``` source
enum CGEventType
```

## Overview

These constants are used:

- In the functions tapCreate(tap:place:options:eventsOfInterest:callback:userInfo:) and tapCreateForPSN(processSerialNumber:place:options:eventsOfInterest:callback:userInfo:) to specify the events of interest for the new event tap.

- To indicate the event type passed to your event tap callback function.

- In the function init(mouseEventSource:mouseType:mouseCursorPosition:mouseButton:) to specify the type of mouse event.

- In the functions type and CGEventSetType to identify the event type.

- In the functions counterForEventType(_:eventType:) and secondsSinceLastEventType(_:eventType:) to indicate the event type.

Note that tablet devices may generate mouse events with embedded tablet data, or tablet pointer and proximity events. Tablet mouse events allow tablets to be used with applications that are not tablet-aware.

## Topics

### Constants

case null

Specifies a null event.

case leftMouseDown

Specifies a mouse down event with the left button.

case leftMouseUp

Specifies a mouse up event with the left button.

case rightMouseDown

Specifies a mouse down event with the right button.

case rightMouseUp

Specifies a mouse up event with the right button.

case mouseMoved

Specifies a mouse moved event.

case leftMouseDragged

Specifies a mouse drag event with the left button down.

case rightMouseDragged

Specifies a mouse drag event with the right button down.

case keyDown

Specifies a key down event.

case keyUp

Specifies a key up event.

case flagsChanged

Specifies a key changed event for a modifier or status key.

case scrollWheel

Specifies a scroll wheel moved event.

case tabletPointer

Specifies a tablet pointer event.

case tabletProximity

Specifies a tablet proximity event.

case otherMouseDown

Specifies a mouse down event with one of buttons 2-31.

case otherMouseUp

Specifies a mouse up event with one of buttons 2-31.

case otherMouseDragged

Specifies a mouse drag event with one of buttons 2-31 down.

case tapDisabledByTimeout

Specifies an event indicating the event tap is disabled because of timeout.

case tapDisabledByUserInput

Specifies an event indicating the event tap is disabled because of user input.

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

enum CGEventSuppressionState

Specify the event suppression states that can occur after posting an event.

enum CGEventTapLocation

Constants that specify possible tapping points for events.

