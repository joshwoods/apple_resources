

- SensorKit
- SRSensorReader
-  sensor 

Instance Property

# sensor

The particular sensor that this object reads.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var sensor: SRSensor { get }
```

## Discussion

The framework sets this property to the sensor you pass into init(sensor:).

## See Also

### Creating a sensor reader

init(sensor: SRSensor)

Initializes a new sensor reader object.

struct SRSensor

The sensors an app can read.

