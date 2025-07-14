

- SensorKit
- SRSensor
-  keyboardMetrics 

Type Property

# keyboardMetrics

A sensor that provides information about keyboard usage.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
static let keyboardMetrics: SRSensor
```

## Discussion

The sample type for this sensor is SRKeyboardMetrics.

You need to provide a reason to record keyboard metrics by adding the SRSensorUsageKeyboardMetrics dictionary to the NSSensorKitUsageDetail key in the information property list.

## See Also

### Reading device sensors

static let deviceUsageReport: SRSensor

A sensor that provides information about device usage.

static let onWristState: SRSensor

A sensor that describes the watch’s position on the wrist.

