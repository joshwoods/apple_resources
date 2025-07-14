

- Core Graphics
-  CGError 

Enumeration

# CGError

A uniform type for result codes returned by functions in Core Graphics.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CGError
```

## Topics

### Constants

case cannotComplete

The requested operation is inappropriate for the parameters passed in, or the current system state.

case failure

A general failure occurred.

case illegalArgument

One or more of the parameters passed to a function are invalid. Check for `NULL` pointers.

case invalidConnection

The parameter representing a connection to the window server is invalid.

case invalidContext

The `CPSProcessSerNum` or context identifier parameter is not valid.

case invalidOperation

The requested operation is not valid for the parameters passed in, or the current system state.

case noneAvailable

The requested operation could not be completed as the indicated resources were not found.

case notImplemented

Return value from obsolete function stubs present for binary compatibility, but not typically called.

case rangeCheck

A parameter passed in has a value that is inappropriate, or which does not map to a useful operation or value.

case success

The requested operation was completed successfully.

case typeCheck

A data type or token was encountered that did not match the expected type or token.

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

### Related Documentation

Quartz 2D Programming Guide

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

