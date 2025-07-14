

- SensorKit
- SRSensor
-  ambientPressure 

Type Property

# ambientPressure

A sensor that provides pressure and temperature metrics.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
static let ambientPressure: SRSensor
```

## Discussion

The sample type for this sensor is `[`CMRecordedPressureData`]`.

You need to provide a reason to record ambient pressure by adding the SRSensorUsageElevation dictionary to the NSSensorKitUsageDetail key in the information property list.

## See Also

### Reading environment sensors

static let ambientLightSensor: SRSensor

A sensor that provides ambient light information.

