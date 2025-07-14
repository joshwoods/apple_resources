

- Core Motion
- CMWaterSubmersionMeasurement
-  CMWaterSubmersionMeasurement.DepthState 

Enumeration

# CMWaterSubmersionMeasurement.DepthState

A state based on the device’s depth under water.

iOS 4.0+iPadOS 4.0+visionOS 1.0+watchOS 2.0+

``` source
enum DepthState
```

## Topics

### Depth states

case notSubmerged

The device is not submerged in water.

case submergedShallow

The device is submerged, but less than 1 meter under water.

case submergedDeep

The device is submerged at least 1 meter under water.

case approachingMaxDepth

The device is approaching the maximum safe diving depth.

case pastMaxDepth

The device has exceeded the maximum safe diving depth.

case sensorDepthError

An error with the depth sensor occurred.

case unknown

The device’s depth state is unknown.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing the data

var date: Date

The time and date when the system recorded the measurements.

var depth: Measurement&lt;UnitLength>?

The depth under water.

var pressure: Measurement&lt;UnitPressure>?

The water pressure.

var surfacePressure: Measurement&lt;UnitPressure>

The surface air pressure.

var submersionState: CMWaterSubmersionMeasurement.DepthState

The depth state.

