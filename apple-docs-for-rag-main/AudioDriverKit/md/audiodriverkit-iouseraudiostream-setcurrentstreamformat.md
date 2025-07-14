

- AudioDriverKit
- IOUserAudioStream
-  SetCurrentStreamFormat 

Instance Method

# SetCurrentStreamFormat

Sets the current stream format to a given audio stream basic description.

DriverKit 21.0+

``` source
kern_return_t SetCurrentStreamFormat(const IOUserAudioStreamBasicDescription * in_format);
```

## Parameters 

`in_format`  

A pointer to an `IOIUserAudioStreamBasicDescription` to use as the new format.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If successful, changing the format sends a notification to the host to update the object state.

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Stream Formats

GetCurrentStreamFormat

Returns the current stream format, as an audio stream basic description.

SetAvailableStreamFormats

Sets the available stream formats to an array of audio stream basic descriptions.

GetAvailableStreamFormats

Returns the available stream formats as an array of audio stream basic descriptions.

GetNumberAvailableStreamFormats

Returns the number of available stream formats.

IOUserAudioStreamBasicDescription

A structure that encapsulates all of the information for describing the basic format properties of a stream of audio data.

GetStreamDirection

Gets the direction of the stream: input or output.

IOUserAudioStreamDirection

A type representing the direction of audio flow.

SetStreamIsActive

Sets a Boolean value that indicates whether the stream is active and doing I/O.

GetStreamIsActive

Gets a value that indicates whether the stream is active and doing I/O.

