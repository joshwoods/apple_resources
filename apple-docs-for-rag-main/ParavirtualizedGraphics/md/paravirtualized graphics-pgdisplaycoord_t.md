

- Paravirtualized Graphics
-  PGDisplayCoord_t 

Structure

# PGDisplayCoord_t

Coordinates that describe sizes or offsets within a 2D array of pixels.

Mac Catalyst 14.0+macOS 11.0+

``` source
struct PGDisplayCoord_t
```

## Topics

### Creating Display Coordinates

init()

Initializes a default display coordinate.

init(x: UInt16, y: UInt16)

Initializes a coordinate.

### Inspecting Coordinate Values

var x: UInt16

The horizontal coordinate value.

var y: UInt16

The vertical coordinate value.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Displays

class PGDisplayDescriptor

A descriptor for a virtual display.

protocol PGDisplay

An object that provides display functionality to the guest operating system in a way that the host-side virtual machine app can intercept.

class PGDisplayMode

A description of a supported display mode.

