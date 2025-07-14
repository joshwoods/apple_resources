

- HealthKit
- HKHeartbeatSeriesBuilder
-  init(healthStore:device:start:) 

Initializer

# init(healthStore:device:start:)

Creates a new heartbeat series builder.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    healthStore: HKHealthStore,
    device: HKDevice?,
    start startDate: Date
)
```

## Parameters 

`healthStore`  

The HealthKit store.

`device`  

An object representing the device that provided the heartbeat data. Pass `nil` if the app is generating its own data.

`startDate`  

The sample’s start date.

## See Also

### Creating a Heartbeat Series Builder

class var maximumCount: Int

The maximum number of heartbeats you can add to the sample.

