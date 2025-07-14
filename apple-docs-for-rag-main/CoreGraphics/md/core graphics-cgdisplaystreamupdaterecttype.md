

- Core Graphics
-  CGDisplayStreamUpdateRectType 

Enumeration

# CGDisplayStreamUpdateRectType

Use these constants to determine which rectangles your app is interested in.

Mac CatalystmacOS

``` source
enum CGDisplayStreamUpdateRectType
```

## Topics

### Constants

case refreshedRects

The rectangles for the portions of the display that were redrawn.

case movedRects

The rectangles for the portions of the display that were simply moved from one part of the display to another.

case dirtyRects

The union of both rectangles that were redrawn and rectangles that were moved.

case reducedDirtyRects

The union is calculated and then simplified. This reduces the number of rectangles returned to your app, but it may report some pixels that were not actually changed.

### Initializers

init?(rawValue: Int32)

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

enum CGEventTapOptions

Constants that specify whether a new event tap is an active filter or a passive listener.

