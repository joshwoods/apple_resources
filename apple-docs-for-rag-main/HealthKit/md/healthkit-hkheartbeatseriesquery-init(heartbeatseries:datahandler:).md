

- HealthKit
- HKHeartbeatSeriesQuery
-  init(heartbeatSeries:dataHandler:) 

Initializer

# init(heartbeatSeries:dataHandler:)

Creates a new heartbeat series query.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
init(
    heartbeatSeries: HKHeartbeatSeriesSample,
    dataHandler: @escaping (HKHeartbeatSeriesQuery, TimeInterval, Bool, Bool, (any Error)?) -> Void
)
```

## Parameters 

`heartbeatSeries`  

The series sample containing the heartbeat data.

`dataHandler`  

The handler called by the query. The handler takes the following parameters:

`query`  
The query that returned the heartbeat data.

`timeSinceSeriesStart`  
The time of the heartbeat, measured from the series builder’s start date. This must be a positive value.

`precededByGap`  
A Boolean value that indicates whether this heartbeat was immediately preceded by a gap in the data, indicating that one or more heartbeats may be missing.

`done`  
A Boolean value that indicates whether the query is complete.

`error`  
If an error occurred, this contains an object that describes the error; otherwise, `nil`.

## Discussion

The system calls the `dataHandler` once for each heartbeat until either the `done` parameter is true, or you call stop(_:).

