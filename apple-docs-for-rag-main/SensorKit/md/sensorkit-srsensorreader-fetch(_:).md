

- SensorKit
- SRSensorReader
-  fetch(\_:) 

Instance Method

# fetch(\_:)

Fetches the samples that a fetch request specifies.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func fetch(_ request: SRFetchRequest)
```

## Parameters 

`request`  

An object that describes the device from which to retrieve samples, and samaple age of interest.

## Discussion

An app calls this function to access data for the caller’s sensor.

Upon success, the framework delivers results in the form of *samples* via the delegate’s sensorReader(_:fetching:didFetchResult:) callback. The framework invokes the delegate multiple times if this function results in multiple samples.

The framework returns sensor data only for the argument fetch-object’s device, and that’s dated only within the argument fetch-object’s time window. Within that window, this function returns only the data that the framework recorded (see startRecording()), and that the framework hasn’t deleted (see SRDeletionRecord).

## See Also

### Reading recorded data

func fetchDevices()

Acquires device information for all devices that store data for this reader’s sensor.

class SRDevice

A representation of a device that provides sample data.

