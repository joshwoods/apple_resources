

- SensorKit
- SRSensor
-  ambientLightSensor 

Type Property

# ambientLightSensor

A sensor that provides ambient light information.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
static let ambientLightSensor: SRSensor
```

## Discussion

The sample type for this sensor is SRAmbientLightSample.

You need to provide a reason to record ambient light by adding the SRSensorUsageAmbientLightSensor dictionary to the NSSensorKitUsageDetail key in the information property list.

## See Also

### Reading environment sensors

static let ambientPressure: SRSensor

A sensor that provides pressure and temperature metrics.

