

- SensorKit
- SRSensor
-  phoneUsageReport 

Type Property

# phoneUsageReport

A sensor that reports the amount of time that the user is on phone calls.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
static let phoneUsageReport: SRSensor
```

## Discussion

The sample type for this sensor is SRPhoneUsageReport.

You need to provide a reason to record phone usage by adding the SRSensorUsagePhoneUsage dictionary to the NSSensorKitUsageDetail key in the information property list.

## See Also

### Reading app activity sensors

static let messagesUsageReport: SRSensor

A sensor that provides information about use of the Messages app.

