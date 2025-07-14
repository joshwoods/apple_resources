

- HealthKit
- HKHeartbeatSeriesBuilder
-  addMetadata(\_:completion:) 

Instance Method

# addMetadata(\_:completion:)

Adds metadata to the sample.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func addMetadata(
    _ metadata: [String : Any],
    completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func addMetadata(_ metadata: [String : Any]) async throws
```

## Parameters 

`metadata`  

The metadata dictionary contains extra information describing all the samples created by the builder. The dictionary’s keys are all strings. The values may be strings, numbers, or date objects. For a complete list of predefined metadata keys, see Metadata Keys.

Using predefined keys helps facilitate sharing data between apps; however, you are also encouraged to create your own, custom keys as needed to extend the samples’ capabilities.

`completion`  

The completion handler called by the builder after it attempts to add the metadata to the series. The completion handler takes the following parameters:

`success`  
A Boolean value that indicates whether the builder successfully added the heartbeat.

`error`  
If the `success` parameter is false, this contains an object that describes the error; otherwise, `nil`.

## Discussion

The builder adds the metadata to the resulting series sample. It incorporates new data using addEntries(from:).

## See Also

### Adding Data

func addHeartbeatWithTimeInterval(sinceSeriesStartDate: TimeInterval, precededByGap: Bool, completion: (Bool, (any Error)?) -> Void)

Adds a heartbeat to the series.

