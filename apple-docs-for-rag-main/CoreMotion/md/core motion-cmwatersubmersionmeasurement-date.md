

- Core Motion
- CMWaterSubmersionMeasurement
-  date 

Instance Property

# date

The time and date when the system recorded the measurements.

iOS 16.0+iPadOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var date: Date { get }
```

## See Also

### Accessing the data

var depth: Measurement&lt;UnitLength>?

The depth under water.

var pressure: Measurement&lt;UnitPressure>?

The water pressure.

var surfacePressure: Measurement&lt;UnitPressure>

The surface air pressure.

var submersionState: CMWaterSubmersionMeasurement.DepthState

The depth state.

enum DepthState

A state based on the device’s depth under water.

