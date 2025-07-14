

- AudioDriverKit
- IOUserAudioClockDevice
-  init 

Instance Method

# init

Initializes an instance of the audio clock device class.

DriverKit 21.0+

``` source
bool init(IOUserAudioDriver * in_driver, bool in_supports_prewarming, OSString * in_device_uid, OSString * in_model_uid, OSString * in_manufacturer_uid, uint32_t in_zero_timestamp_period);
```

## Parameters 

`in_driver`  

The IOUserAudioDriver that owns this object.

`in_supports_prewarming`  

A Boolean value that specifies whether the device supports prewarming I/O.

`in_device_uid`  

A pointer to an OSString containing the device UID.

`in_model_uid`  

A pointer to an OSString containing the model UID.

`in_manufacturer_uid`  

A pointer to an OSString containing the manufacturer UID.

`in_zero_timestamp_period`  

A uint32_t whose value indicates the number of sample frames the host can expect between successive timestamps returned from GetZeroTimestampPeriod. In other words, if GetZeroTimestampPeriod returns a sample time of `x`, the host can expect that the next valid timestamp it receives will be `x + in_zero_timestamp_period`.

## Return Value

`true` if initialization succeeded; `false` otherwise.

## See Also

### Creating a Clock Device

Create

Allocates and initializes an instance of the audio clock device class.

IOUserAudioDriver

A DriverKit provider object that manages communications with an audio device.

