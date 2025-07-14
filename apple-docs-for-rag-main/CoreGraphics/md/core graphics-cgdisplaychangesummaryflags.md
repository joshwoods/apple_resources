

- Core Graphics
-  CGDisplayChangeSummaryFlags 

Structure

# CGDisplayChangeSummaryFlags

The configuration parameters that are passed to a display reconfiguration callback function.

Mac CatalystmacOS

``` source
struct CGDisplayChangeSummaryFlags
```

## Overview

For information about how these constants are used, see the callback CGDisplayReconfigurationCallBack.

## Topics

### Constants

static var beginConfigurationFlag: CGDisplayChangeSummaryFlags

The display configuration is about to change.

static var movedFlag: CGDisplayChangeSummaryFlags

The location of the upper-left corner of the display in the global display coordinate space has changed.

static var setMainFlag: CGDisplayChangeSummaryFlags

The display is now the main display.

static var setModeFlag: CGDisplayChangeSummaryFlags

The display mode has changed.

static var addFlag: CGDisplayChangeSummaryFlags

The display has been added to the active display list.

static var removeFlag: CGDisplayChangeSummaryFlags

The display has been removed from the active display list.

static var enabledFlag: CGDisplayChangeSummaryFlags

The display has been enabled.

static var disabledFlag: CGDisplayChangeSummaryFlags

The display has been disabled.

static var mirrorFlag: CGDisplayChangeSummaryFlags

The display is now mirroring another display.

static var unMirrorFlag: CGDisplayChangeSummaryFlags

The display is no longer mirroring another display.

static var desktopShapeChangedFlag: CGDisplayChangeSummaryFlags

### Initializers

init(rawValue: UInt32)

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

