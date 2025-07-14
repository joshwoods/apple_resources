

- AudioDriverKit
- IOUserAudioStream
-  GetAvailableStreamFormats 

Instance Method

# GetAvailableStreamFormats

Returns the available stream formats as an array of audio stream basic descriptions.

DriverKit 21.0+

``` source
size_t GetAvailableStreamFormats(IOUserAudioStreamBasicDescription * out_formats, size_t in_num_formats);
```

## Parameters 

`out_formats`  

A pointer to a buffer of type `IOUserAudioStreamBasicDescription`, with a size of `in_num_formats`. On return, this buffer contains the available formats.

`in_num_formats`  

The size of the `out_formats` buffer.

## Return Value

The number of descriptions populated in the `out_formats` buffer.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Stream Formats

SetCurrentStreamFormat

Sets the current stream format to a given audio stream basic description.

GetCurrentStreamFormat

Returns the current stream format, as an audio stream basic description.

SetAvailableStreamFormats

Sets the available stream formats to an array of audio stream basic descriptions.

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

