

- SensorKit
- SRSensorReaderDelegate
-  sensorReader(\_:didFetch:) 

Instance Method

# sensorReader(\_:didFetch:)

Provides the delegate with one or more devices.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
optional func sensorReader(
    _ reader: SRSensorReader,
    didFetch devices: [SRDevice]
)
```

## Parameters 

`reader`  

The sensor reader that fetched the device(s).

`devices`  

The fetched devices.

## See Also

### Fetching Devices

func sensorReader(SRSensorReader, fetchDevicesDidFailWithError: any Error)

Provides the delegate a reason when the reader fails to fetch devices.

class SRDevice

A representation of a device that provides sample data.

