

- AudioDriverKit
- IOUserAudioBox
-  Create 

Static Method

# Create

Allocates and initializes an instance of the audio box class.

DriverKit 21.0+

``` source
static OSSharedPtr Create(IOUserAudioDriver * in_driver, bool in_is_acquirable, OSString * in_box_uid);
```

## Parameters 

`in_driver`  

The IOUserAudioDriver that owns this object.

`in_is_acquirable`  

A Boolean value that specifies if the box supports being acquired.

`in_box_uid`  

The name of the box, as an OSString.

## Return Value

A poiner to an IOUserAudioBox, if allocation and initialization succeeded.

## Discussion

If you subclass IOUserAudioBox to override this class’ behavior, don’t use Create to allocate and initialize the custom subclass.

## See Also

### Creating an Audio Box

init

Initializes an instance of the audio box class.

IOUserAudioDriver

A DriverKit provider object that manages communications with an audio device.

