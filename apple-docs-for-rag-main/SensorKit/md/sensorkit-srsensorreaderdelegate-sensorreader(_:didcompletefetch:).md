

- SensorKit
- SRSensorReaderDelegate
-  sensorReader(\_:didCompleteFetch:) 

Instance Method

# sensorReader(\_:didCompleteFetch:)

Provides the delegate with a completed fetch request.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
optional func sensorReader(
    _ reader: SRSensorReader,
    didCompleteFetch fetchRequest: SRFetchRequest
)
```

## Parameters 

`reader`  

The reader that completed the fetch request.

`fetchRequest`  

The completed fetch request.

## See Also

### Reading Recorded Data

func sensorReader(SRSensorReader, fetching: SRFetchRequest, didFetchResult: SRFetchResult&lt;AnyObject>) -> Bool

Provides the delegate with a fetch result.

func sensorReader(SRSensorReader, fetching: SRFetchRequest, failedWithError: any Error)

Provides the delegate with a fetch failure reason.

