

- AudioDriverKit
- IOUserAudioDevice
-  AddStream 

Instance Method

# AddStream

Adds an audio stream to the device.

DriverKit 21.0+

``` source
kern_return_t AddStream(IOUserAudioStream * in_stream);
```

## Parameters 

`in_stream`  

The stream to add to the device.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If adding the stream succeeds, the stream’s reference count increments by one.

## See Also

### Working with Audio Streams

RemoveStream

Removes an audio stream from the device.

IOUserAudioStream

An audio object that performs I/O for an audio device.

