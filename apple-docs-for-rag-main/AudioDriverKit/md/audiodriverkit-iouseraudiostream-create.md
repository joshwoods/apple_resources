

- AudioDriverKit
- IOUserAudioStream
-  Create 

Static Method

# Create

Allocates and initializes an instance of the audio stream class.

DriverKit 21.0+

``` source
static OSSharedPtr Create(IOUserAudioDriver * in_driver, IOUserAudioStreamDirection in_direction, IOMemoryDescriptor * in_io_memory_descriptor);
```

## Parameters 

`in_driver`  

The IOUserAudioDriver that owns this object.

`in_direction`  

A `IOUserAudioStreamDirection` for the stream’s direction: input or output.

`in_io_memory_descriptor`  

A pointer to a IOMemoryDescriptor. The stream maps the descriptor’s buffer to the host for doing audio I/O.

## Return Value

A poiner to an IOUserAudioStream, if allocation and initialization succeeded.

## Discussion

If you subclass IOUserAudioStream to override this class’ behavior, don’t use Create to allocate and initialize the custom subclass.

## See Also

### Creating an Audio Stream

init

Initializes an instance of the audio stream class.

IOUserAudioDriver

A DriverKit provider object that manages communications with an audio device.

