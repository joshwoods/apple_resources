

- SensorKit
- SRSensorReaderDelegate
-  sensorReader(\_:fetchDevicesDidFailWithError:) 

Instance Method

# sensorReader(\_:fetchDevicesDidFailWithError:)

Provides the delegate a reason when the reader fails to fetch devices.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
optional func sensorReader(
    _ reader: SRSensorReader,
    fetchDevicesDidFailWithError error: any Error
)
```

## Parameters 

`reader`  

The reader that failed to fetch devices.

`error`  

An object that describes the cause of failure.

## See Also

### Fetching Devices

func sensorReader(SRSensorReader, didFetch: [SRDevice])

Provides the delegate with one or more devices.

class SRDevice

A representation of a device that provides sample data.

