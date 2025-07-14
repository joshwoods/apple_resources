

- SensorKit
- SRSensorReader
-  fetchDevices() 

Instance Method

# fetchDevices()

Acquires device information for all devices that store data for this reader’s sensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func fetchDevices()
```

## Discussion

Upon success, the framework provides an array of devices to the delegate via sensorReader(_:didFetch:). Upon failure, the framework invokes the delegate’s sensorReader(_:fetchDevicesDidFailWithError:) callback.

## See Also

### Reading recorded data

func fetch(SRFetchRequest)

Fetches the samples that a fetch request specifies.

class SRDevice

A representation of a device that provides sample data.

