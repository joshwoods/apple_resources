

- Core Graphics
-  CGConfigureOption 

Structure

# CGConfigureOption

The scope of the changes in a display configuration transaction.

Mac CatalystmacOS

``` source
struct CGConfigureOption
```

## Overview

For information about how these constants are used, see the function CGCompleteDisplayConfiguration(_:_:).

## Topics

### Initializers

init(rawValue: UInt32)

### Type Properties

static var forAppOnly: CGConfigureOption

Changes persist for the lifetime of the current application. After the application terminates, the display configuration settings revert to the current login session.

static var forSession: CGConfigureOption

Changes persist for the lifetime of the current login session. After the current session terminates, the displays revert to the last saved permanent configuration.

static var permanently: CGConfigureOption

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Enumerations

struct CGCaptureOptions

Configuration parameters that are used when capturing displays.

enum CGColorConversionInfoTransformType

Constants describing how a color conversion uses color spaces.

enum CGColorRenderingIntent

Handling options for colors that are not located within the destination color space of a graphics context.

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

enum CGEventTapOptions

Constants that specify whether a new event tap is an active filter or a passive listener.

