

- Core Graphics
-  CGWindowImageOption 

Structure

# CGWindowImageOption

The data type to use to specify the type of image to be generated for a window.

Mac CatalystmacOS

``` source
struct CGWindowImageOption
```

## Overview

This type is used in conjunction with the constants described in Window Image Types.

## Topics

### Initializers

init(rawValue: UInt32)

### Type Properties

static var bestResolution: CGWindowImageOption

When capturing the window, return the best image resolution. The returned image size may be different than the screen size.

static var boundsIgnoreFraming: CGWindowImageOption

static var nominalResolution: CGWindowImageOption

When capturing the window, return the nominal image resolution. The returned image size is the same as the screen size.

static var onlyShadows: CGWindowImageOption

static var shouldBeOpaque: CGWindowImageOption

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

