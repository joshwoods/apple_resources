

- Spatial
-  Axis3D 

Structure

# Axis3D

Constants that describe an axis.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct Axis3D
```

## Topics

### Constants

static var x: Axis3D

The operation is along the x-axis.

static var y: Axis3D

The operation is along the y-axis.

static var z: Axis3D

### Initializers

init(UInt32)

Creates a new 3D axis structure.

init(rawValue: UInt32)

Creates a new instance with the specified raw value.

### Inspecting the axis

var rawValue: UInt32

The corresponding value of the raw type.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Data structures

struct Vector3D

A three-element vector.

