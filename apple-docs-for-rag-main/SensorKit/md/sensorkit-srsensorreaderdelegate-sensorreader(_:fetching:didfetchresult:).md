

- SensorKit
- SRSensorReaderDelegate
-  sensorReader(\_:fetching:didFetchResult:) 

Instance Method

# sensorReader(\_:fetching:didFetchResult:)

Provides the delegate with a fetch result.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
optional func sensorReader(
    _ reader: SRSensorReader,
    fetching fetchRequest: SRFetchRequest,
    didFetchResult result: SRFetchResult
) -> Bool
```

## Parameters 

`reader`  

The sensor reader for which the fetch provides results.

`fetchRequest`  

The completed fetch request.

`result`  

The fetch request’s result.

## Discussion

The framework expects the app to know the result’s type based on the reader’s sensor. To see a list of result types per sensor, see Sample types.

When a fetch produces multiple results, the framework invokes this callback once for each result.

To reuse a fetch result within the scope of this function, create a copy of `fetchResult` rather than assigning a strong reference to it.

## See Also

### Reading Recorded Data

func sensorReader(SRSensorReader, didCompleteFetch: SRFetchRequest)

Provides the delegate with a completed fetch request.

func sensorReader(SRSensorReader, fetching: SRFetchRequest, failedWithError: any Error)

Provides the delegate with a fetch failure reason.

