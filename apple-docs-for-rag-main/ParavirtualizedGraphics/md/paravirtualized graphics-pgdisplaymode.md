

- Paravirtualized Graphics
-  PGDisplayMode 

Class

# PGDisplayMode

A description of a supported display mode.

Mac Catalyst 14.0+macOS 11.0+

``` source
class PGDisplayMode
```

## Topics

### Creating a Display Mode

init?(sizeInPixels: PGDisplayCoord_t, refreshRateInHz: Double)

Creates a new display mode.

### Inspecting Mode Properties

var sizeInPixels: PGDisplayCoord_t

The display mode’s dimensions in pixels.

var refreshRate: Double

The mode’s refresh rate.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Displays

class PGDisplayDescriptor

A descriptor for a virtual display.

protocol PGDisplay

An object that provides display functionality to the guest operating system in a way that the host-side virtual machine app can intercept.

struct PGDisplayCoord_t

Coordinates that describe sizes or offsets within a 2D array of pixels.

