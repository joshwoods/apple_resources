

- AudioDriverKit
- IOUserAudioDevice
-  RemoveStream 

Instance Method

# RemoveStream

Removes an audio stream from the device.

DriverKit 21.0+

``` source
kern_return_t RemoveStream(IOUserAudioStream * in_stream);
```

## Parameters 

`in_stream`  

The stream to remove from the device.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If removing the stream succeeds, the stream’s reference count decrements by one.

## See Also

### Working with Audio Streams

AddStream

Adds an audio stream to the device.

IOUserAudioStream

An audio object that performs I/O for an audio device.

