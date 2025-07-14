

- SensorKit
- SRSensorReaderDelegate
-  sensorReader(\_:fetching:failedWithError:) 

Instance Method

# sensorReader(\_:fetching:failedWithError:)

Provides the delegate with a fetch failure reason.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
optional func sensorReader(
    _ reader: SRSensorReader,
    fetching fetchRequest: SRFetchRequest,
    failedWithError error: any Error
)
```

## Parameters 

`reader`  

The sensor reader for which the fetch failed.

`fetchRequest`  

The original fetch request.

`error`  

An object that describes the cause of failure.

## See Also

### Reading Recorded Data

func sensorReader(SRSensorReader, fetching: SRFetchRequest, didFetchResult: SRFetchResult&lt;AnyObject>) -> Bool

Provides the delegate with a fetch result.

func sensorReader(SRSensorReader, didCompleteFetch: SRFetchRequest)

Provides the delegate with a completed fetch request.

