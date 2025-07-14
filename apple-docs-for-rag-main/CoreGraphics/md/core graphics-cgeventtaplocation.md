

- Core Graphics
-  CGEventTapLocation 

Enumeration

# CGEventTapLocation

Constants that specify possible tapping points for events.

Mac CatalystmacOS

``` source
enum CGEventTapLocation
```

## Overview

In addition to the three tapping points described above, an event tap may also be placed where annotated events are delivered to a specific application. For more information, see the function tapCreateForPSN(processSerialNumber:place:options:eventsOfInterest:callback:userInfo:).

## Topics

### Constants

case cghidEventTap

Specifies that an event tap is placed at the point where HID system events enter the window server.

case cgSessionEventTap

Specifies that an event tap is placed at the point where HID system and remote control events enter a login session.

case cgAnnotatedSessionEventTap

Specifies that an event tap is placed at the point where session events have been annotated to flow to an application.

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

enum CGEventTapOptions

Constants that specify whether a new event tap is an active filter or a passive listener.

