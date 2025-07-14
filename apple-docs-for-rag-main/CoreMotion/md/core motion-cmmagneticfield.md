

- Core Motion
-  CMMagneticField 

Structure

# CMMagneticField

A structure containing 3-axis magnetometer data

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
struct CMMagneticField
```

## Topics

### Getting the Field Values

var x: Double

X-axis magnetic field in microteslas.

var y: Double

Y-axis magnetic field in microteslas.

var z: Double

Z-axis magnetic field in microteslas.

### Initializers

init()

init(x: Double, y: Double, z: Double)

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Getting the Field Strength

var magneticField: CMMagneticField

Returns the magnetic field measured by the magnetometer.

