

- SensorKit
- SRDeviceUsageReport
- SRDeviceUsageReport.ApplicationUsage
-  relativeStartTime 

Instance Property

# relativeStartTime

The time the user starts the app relative to the start time of the first app in a report interval.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+

``` source
var relativeStartTime: TimeInterval { get }
```

## Discussion

Use this property to order and determine the time between app instances in the same report. The first instance of this property in the report interval is `0`.

## See Also

### Timing App Use

var usageTime: TimeInterval

The amount of time the user uses the app.

