

- Core Graphics
-  CGEventSourceStateID 

Enumeration

# CGEventSourceStateID

Constants that specify the possible source states of an event source.

Mac CatalystmacOS

``` source
enum CGEventSourceStateID
```

## Overview

A source state refers to a global event state table. These tables contain accumulated information on modifier flag state, keyboard key state, mouse button state, and related internal parameters placed in effect by posting events with associated sources.

Two pre-existing event state tables are defined:

- The `kCGEventSourceStateCombinedSessionState` table reflects the combined state of all event sources posting to the current user login session. If your program is posting events from within a login session, you should use this source state when you create an event source.

- The `kCGEventSourceStateHIDSystemState` table reflects the combined state of all hardware event sources posting from the HID system. If your program is a daemon or a user space device driver interpreting hardware state and generating events, you should use this source state when you create an event source.

Specialized applications such as remote control programs may want to generate and track event source state independent of other processes. These programs should use the `kCGEventSourceStatePrivate` value in creating their event source. An independent state table and unique source state ID (`CGEventSourceStateID`) are created to track the event source’s state. This independent state table is owned by the creating event source and released with it.

## Topics

### Constants

case privateState

Specifies that an event source should use a private event state table.

case combinedSessionState

Specifies that an event source should use the event state table that reflects the combined state of all event sources posting to the current user login session.

case hidSystemState

Specifies that an event source should use the event state table that reflects the combined state of all hardware event sources posting from the HID system.

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

enum CGEventSuppressionState

Specify the event suppression states that can occur after posting an event.

enum CGEventTapLocation

Constants that specify possible tapping points for events.

enum CGEventTapOptions

Constants that specify whether a new event tap is an active filter or a passive listener.

