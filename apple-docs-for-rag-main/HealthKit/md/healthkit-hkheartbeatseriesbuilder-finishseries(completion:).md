

- HealthKit
- HKHeartbeatSeriesBuilder
-  finishSeries(completion:) 

Instance Method

# finishSeries(completion:)

Finalizes the series and returns the resulting heartbeat series sample.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func finishSeries(completion: @escaping (HKHeartbeatSeriesSample?, (any Error)?) -> Void)
```

``` source
func finishSeries() async throws -> HKHeartbeatSeriesSample
```

## Parameters 

`completion`  

The completion handler called by the builder after it attempts to create and save the heartbeat series sample. The completion handler takes the following parameters:

`heartbeatSeries`  
If successful it contains the resuting sample; otherwise, `nil`.

`error`  
If an error occurs, this contains an object that describes the error; otherwise, `nil`.

## Discussion

Call finishSeries(completion:) after inserting all the heartbeats for the series. The series builder creates the series sample, saves it to the HealthKit store, and passes it to the completion handler.

Calling this method before inserting any heartbeats results in an error. Also, calling this method invalidates the series builder; you cannot call any other series builder methods after calling this method.

