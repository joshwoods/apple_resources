

- SensorKit
- SRSensorReaderDelegate
-  sensorReader(\_:didChange:) 

Instance Method

# sensorReader(\_:didChange:)

Notifies the delegate of the reader’s new authorization status.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
optional func sensorReader(
    _ reader: SRSensorReader,
    didChange authorizationStatus: SRAuthorizationStatus
)
```

## Parameters 

`reader`  

The sensor reader whose authorization state changed.

`authorizationStatus`  

A flag indicating whether the framework authorizes the sensor reader.

