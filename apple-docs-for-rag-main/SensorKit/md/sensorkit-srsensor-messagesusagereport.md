

- SensorKit
- SRSensor
-  messagesUsageReport 

Type Property

# messagesUsageReport

A sensor that provides information about use of the Messages app.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
static let messagesUsageReport: SRSensor
```

## Discussion

The sample type for this sensor is SRMessagesUsageReport.

You need to provide a reason to record Messages app usage by adding the SRSensorUsageMessageUsage dictionary to the NSSensorKitUsageDetail key in the information property list.

## See Also

### Reading app activity sensors

static let phoneUsageReport: SRSensor

A sensor that reports the amount of time that the user is on phone calls.

