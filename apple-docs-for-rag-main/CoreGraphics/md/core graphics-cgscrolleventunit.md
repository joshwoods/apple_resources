

- Core Graphics
-  CGScrollEventUnit 

Enumeration

# CGScrollEventUnit

Constants that specify the unit of measurement for a scrolling event.

Mac CatalystmacOS

``` source
enum CGScrollEventUnit
```

## Overview

You may pass one of these constants to the function CGEventCreateScrollWheelEvent to specify the unit of measurement for the event. The constant `kCGScrollEventUnitPixel` produces an event that most applications interpret as a smooth scrolling event. By default, the scale is about ten pixels per line. You can alter the scale with the function CGEventSourceSetPixelsPerLine.

## Topics

### Constants

case pixel

Specifies that the unit of measurement is pixels.

case line

Specifies that the unit of measurement is lines.

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

