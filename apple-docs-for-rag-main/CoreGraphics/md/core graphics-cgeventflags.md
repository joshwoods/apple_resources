

- Core Graphics
-  CGEventFlags 

Structure

# CGEventFlags

Constants that indicate the modifier key state at the time an event is created, as well as other event-related states.

Mac CatalystmacOS

``` source
struct CGEventFlags
```

## Overview

These constants specify masks for the bits in an event flags bit mask. Event flags indicate the modifier key state at the time an event is created, as well as other event-related states. Event flags are used in accessor functions such as flags, CGEventSetFlags, and flagsState(_:).

## Topics

### Constants

static var maskAlphaShift: CGEventFlags

Indicates that the Caps Lock key is down for a keyboard, mouse, or flag-changed event.

static var maskShift: CGEventFlags

Indicates that the Shift key is down for a keyboard, mouse, or flag-changed event.

static var maskControl: CGEventFlags

Indicates that the Control key is down for a keyboard, mouse, or flag-changed event.

static var maskAlternate: CGEventFlags

Indicates that the Alt or Option key is down for a keyboard, mouse, or flag-changed event.

static var maskCommand: CGEventFlags

Indicates that the Command key is down for a keyboard, mouse, or flag-changed event.

static var maskHelp: CGEventFlags

Indicates that the Help modifier key is down for a keyboard, mouse, or flag-changed event. This key is not present on most keyboards, and is different than the Help key found in the same row as Home and Page Up.

static var maskSecondaryFn: CGEventFlags

Indicates that the Fn (Function) key is down for a keyboard, mouse, or flag-changed event. This key is found primarily on laptop keyboards.

static var maskNumericPad: CGEventFlags

Identifies key events from the numeric keypad area on extended keyboards.

static var maskNonCoalesced: CGEventFlags

Indicates that mouse and pen movement events are not being coalesced.

### Initializers

init(rawValue: UInt64)

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

