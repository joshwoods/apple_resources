

- SensorKit
- SRSensor
-  onWristState 

Type Property

# onWristState

A sensor that describes the watch’s position on the wrist.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
static let onWristState: SRSensor
```

## Discussion

The sample type for this sensor is SRWristDetection

You need to provide a reason to detect the watch position by adding the SRSensorUsageWristDetection dictionary to the NSSensorKitUsageDetail key in the information property list.

## See Also

### Reading device sensors

static let deviceUsageReport: SRSensor

A sensor that provides information about device usage.

static let keyboardMetrics: SRSensor

A sensor that provides information about keyboard usage.

