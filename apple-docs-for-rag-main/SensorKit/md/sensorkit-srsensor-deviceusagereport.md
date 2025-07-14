

- SensorKit
- SRSensor
-  deviceUsageReport 

Type Property

# deviceUsageReport

A sensor that provides information about device usage.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
static let deviceUsageReport: SRSensor
```

## Discussion

The sample type for this sensor is SRDeviceUsageReport.

You need to provide a reason to record the device usage by adding the SRSensorUsageDeviceUsage dictionary to the NSSensorKitUsageDetail key in the information property list.

## See Also

### Reading device sensors

static let keyboardMetrics: SRSensor

A sensor that provides information about keyboard usage.

static let onWristState: SRSensor

A sensor that describes the watch’s position on the wrist.

