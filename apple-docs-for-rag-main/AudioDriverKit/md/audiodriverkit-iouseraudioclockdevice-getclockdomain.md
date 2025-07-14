

- AudioDriverKit
- IOUserAudioClockDevice
-  GetClockDomain 

Instance Method

# GetClockDomain

Gets the clock domain value of the clock device.

DriverKit 21.0+

``` source
uint32_t GetClockDomain();
```

## Return Value

The clock domain value of the clock device.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Clock Domain

SetClockDomain

Sets the clock domain value of the clock device.

