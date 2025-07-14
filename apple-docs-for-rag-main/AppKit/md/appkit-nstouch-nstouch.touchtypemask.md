

- AppKit
- NSTouch
-  NSTouch.TouchTypeMask 

Structure

# NSTouch.TouchTypeMask

A bit mask identifying a direct or indirect touch type.

macOS 10.12.2+

``` source
struct TouchTypeMask
```

## Topics

### Creating a Touch Type Mask

init(type: NSTouch.TouchType)

Creates a new touch type mask from the touch type.

init(rawValue: UInt)

Creates a new touch type mask from the given raw value.

### Masking the Touch Types

static var direct: NSTouch.TouchTypeMask

A direct touch from a user’s finger on a screen.

static var indirect: NSTouch.TouchTypeMask

An indirect touch that is not on a screen, like a digitizer touch.

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

### Getting the Touch Type

var type: NSTouch.TouchType

A type of touch from a Touch Bar interaction.

enum TouchType

A bit mask identifying a direct or indirect touch type.

