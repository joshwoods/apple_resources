

- Core Motion
- CMWaterSubmersionMeasurement
-  surfacePressure 

Instance Property

# surfacePressure

The surface air pressure.

iOS 16.0+iPadOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var surfacePressure: Measurement { get }
```

## See Also

### Accessing the data

var date: Date

The time and date when the system recorded the measurements.

var depth: Measurement&lt;UnitLength>?

The depth under water.

var pressure: Measurement&lt;UnitPressure>?

The water pressure.

var submersionState: CMWaterSubmersionMeasurement.DepthState

The depth state.

enum DepthState

A state based on the device’s depth under water.

