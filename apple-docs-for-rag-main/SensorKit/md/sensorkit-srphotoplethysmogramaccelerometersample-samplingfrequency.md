

- SensorKit
- SRPhotoplethysmogramAccelerometerSample
-  samplingFrequency 

Instance Property

# samplingFrequency

The frequency of the accelerometer data recording in hertz.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
var samplingFrequency: Measurement { get }
```

## See Also

### Accessing accelerometer data

var nanosecondsSinceStart: Int64

The time in nanoseconds since the start of the accelerometer data recording.

var x: Measurement&lt;UnitAcceleration>

The x-axis acceleration in G’s (gravitational force).

var y: Measurement&lt;UnitAcceleration>

The y-axis acceleration in G’s (gravitational force).

var z: Measurement&lt;UnitAcceleration>

The z-axis acceleration in G’s (gravitational force).

