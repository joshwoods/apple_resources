

- AppKit
-  NSTouch 

Class

# NSTouch

A snapshot of a particular touch at an instant in time.

macOS 10.6+

``` source
class NSTouch
```

## Overview

A touch event is not persistent throughout the touch. A touch creates new instances as it progresses. Use the identity property to follow a specific touch across its lifetime.

Touches do not have a corresponding screen location. The first touch of a touch collection latches to the view underlying the cursor using the same hit detection as mouse events. Additional touches on the same device latch to the same view. Latches remain on views until the user ends a touch or an event cancels it.

## Topics

### Getting the Touch Type

var type: NSTouch.TouchType

A type of touch from a Touch Bar interaction.

enum TouchType

A bit mask identifying a direct or indirect touch type.

struct TouchTypeMask

A bit mask identifying a direct or indirect touch type.

### Using Touch Properties

var identity: any NSCopying &amp; NSObjectProtocol

The changes to a particular touch during its lifetime.

var phase: NSTouch.Phase

The current phase of the touch.

struct Phase

The possible phases of a touch.

var normalizedPosition: NSPoint

The normalized position of the touch.

var isResting: Bool

The indicator for a resting touch.

### Using Touch Device Properties

var device: Any?

The digitizer that generates the touch. Useful to distinguish touches emanating from multiple-device scenarios.

var deviceSize: NSSize

The range of the touch device in points, such as 72 ppi.

### Getting the Touch Location

func location(in: NSView?) -> NSPoint

Indicates the location of the touch in the view’s coordinates.

func previousLocation(in: NSView?) -> NSPoint

Indicates the previous location of the touch in the view’s coordinates.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Mouse, Keyboard, and Touch Events

class NSEvent

An object that contains information about an input action, such as a mouse click or a key press.

