

- AudioDriverKit
- IOUserAudioClockDevice
-  GetUID 

Instance Method

# GetUID

Gets the unique identifier of the clock device.

DriverKit 21.0+

``` source
OSSharedPtr GetUID();
```

## Return Value

A pointer to an OSString containing the UID.

## Discussion

This method synchronizes by using the work queue created by the object.

