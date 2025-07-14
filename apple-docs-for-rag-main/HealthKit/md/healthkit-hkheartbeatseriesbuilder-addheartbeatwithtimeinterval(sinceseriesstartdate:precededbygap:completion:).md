

- HealthKit
- HKHeartbeatSeriesBuilder
-  addHeartbeatWithTimeInterval(sinceSeriesStartDate:precededByGap:completion:) 

Instance Method

# addHeartbeatWithTimeInterval(sinceSeriesStartDate:precededByGap:completion:)

Adds a heartbeat to the series.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func addHeartbeatWithTimeInterval(
    sinceSeriesStartDate timeIntervalSinceStart: TimeInterval,
    precededByGap: Bool,
    completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func addHeartbeat(
    at timeIntervalSinceStart: TimeInterval,
    precededByGap: Bool
) async throws
```

## Parameters 

`timeIntervalSinceStart`  

The time of the heartbeat, measured from the series builder’s start date. This must be a positive value.

`precededByGap`  

A Boolean value that indicates whether this heartbeat was immediately preceded by a gap in the data, indicating that one or more heartbeats may be missing.

`completion`  

The completion handler called by the builder after it attempts to add the heartbeat to the series. The completion handler takes the following parameters:

`success`  
A Boolean value that indicates whether the builder successfully added the heartbeat.

`error`  
If the `success` parameter is false, this contains an object that describes the error; otherwise, `nil`.

## See Also

### Adding Data

func addMetadata([String : Any], completion: (Bool, (any Error)?) -> Void)

Adds metadata to the sample.

