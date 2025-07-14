

- Core Motion
-  CMRotationRate 

Structure

# CMRotationRate

The type of structures representing a measurement of rotation rate.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
struct CMRotationRate
```

## Topics

### Getting the Rotation Rates

var x: Double

The value for the X-axis.

var y: Double

The value for the Y-axis.

var z: Double

The value for the Z-axis.

### Initializers

init()

init(x: Double, y: Double, z: Double)

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Getting the Rotation Rate

var rotationRate: CMRotationRate

The rotation rate as measured by the device’s gyroscope.

class CMRotationRateData

A data object that contains a single rotation-rate measurement.

class CMRecordedRotationRateData

A data object that contains a single rotation-rate measurement at a specific time.

