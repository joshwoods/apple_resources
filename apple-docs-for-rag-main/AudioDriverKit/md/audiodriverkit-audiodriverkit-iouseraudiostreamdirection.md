

- AudioDriverKit
- AudioDriverKit
-  IOUserAudioStreamDirection 

Enumeration

# IOUserAudioStreamDirection

A type representing the direction of audio flow.

DriverKit 21.0+

``` source
enum IOUserAudioStreamDirection : uint32_t;
```

## Discussion

Use `0` for output, and `1` for input.

## Topics

### Enumeration Cases

Input

Output

## See Also

### Working with Stream Formats

SetCurrentStreamFormat

Sets the current stream format to a given audio stream basic description.

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

SetStreamIsActive

Sets a Boolean value that indicates whether the stream is active and doing I/O.

GetStreamIsActive

Gets a value that indicates whether the stream is active and doing I/O.

