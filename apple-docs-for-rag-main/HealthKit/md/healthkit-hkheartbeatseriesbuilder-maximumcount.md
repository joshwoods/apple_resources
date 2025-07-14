

- HealthKit
- HKHeartbeatSeriesBuilder
-  maximumCount 

Type Property

# maximumCount

The maximum number of heartbeats you can add to the sample.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class var maximumCount: Int { get }
```

## Discussion

After reaching the maximum count, any attempt to call the addHeartbeatWithTimeInterval(sinceSeriesStartDate:precededByGap:completion:) method fails.

## See Also

### Creating a Heartbeat Series Builder

init(healthStore: HKHealthStore, device: HKDevice?, start: Date)

Creates a new heartbeat series builder.

