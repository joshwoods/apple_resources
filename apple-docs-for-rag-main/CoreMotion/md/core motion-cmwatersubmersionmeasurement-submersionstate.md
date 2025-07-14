

- Core Motion
- CMWaterSubmersionMeasurement
-  submersionState 

Instance Property

# submersionState

The depth state.

iOS 16.0+iPadOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var submersionState: CMWaterSubmersionMeasurement.DepthState { get }
```

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

enum DepthState

A state based on the device’s depth under water.

