

- AudioDriverKit
- IOUserAudioStream
-  init 

Instance Method

# init

Initializes an instance of the audio stream class.

DriverKit 21.0+

``` source
bool init(IOUserAudioDriver * in_driver, IOUserAudioStreamDirection in_direction, IOMemoryDescriptor * in_io_memory_descriptor);
```

## Parameters 

`in_driver`  

The IOUserAudioDriver that owns this object.

`in_direction`  

A `IOUserAudioStreamDirection` for the stream’s direction: input or output.

`in_io_memory_descriptor`  

A pointer to a IOMemoryDescriptor. The stream maps the descriptor’s buffer to the Host for doing audio I/O.

## Return Value

`true` if initialization succeeded; `false` otherwise.

## See Also

### Creating an Audio Stream

Create

Allocates and initializes an instance of the audio stream class.

IOUserAudioDriver

A DriverKit provider object that manages communications with an audio device.

