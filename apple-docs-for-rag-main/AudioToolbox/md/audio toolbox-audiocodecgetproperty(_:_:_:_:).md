

- Audio Toolbox
-  AudioCodecGetProperty(\_:\_:\_:\_:) 

Function

# AudioCodecGetProperty(\_:\_:\_:\_:)

Retrieves the value of a codec property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func AudioCodecGetProperty(
    _ inCodec: AudioCodec,
    _ inPropertyID: AudioCodecPropertyID,
    _ ioPropertyDataSize: UnsafeMutablePointer,
    _ outPropertyData: UnsafeMutableRawPointer
) -> OSStatus
```

## Parameters 

`inCodec`  

An audio codec object. Because an audio codec object is a Component Manger component instance, you can use the Component Manager (for example, the functions FindNextComponent and OpenAComponent) to obtain an audio codec object.

`inPropertyID`  

Property ID of the property whose value you want to obtain. Codec property IDs are listed in Global Codec Properties and Instance Codec Properties.

`ioPropertyDataSize`  

On input, the size in bytes of the data buffer pointed to by the `outPropertyData` parameter. On output, the amount of data actually written to the buffer.

`outPropertyData`  

The property data buffer.

## Return Value

Returns `NoErr` if successful, otherwise, a result code. See `Result Codes` for a list of possible values.

## Discussion

All property values can be read regardless of the state of the codec. However, the values of some properties depend on whether the codec is initialized. Before calling this function, call the AudioCodecGetPropertyInfo(_:_:_:_:) function to determine the size of buffer you need for the property value.

## See Also

### Accessing Codec Properties

func AudioCodecGetPropertyInfo(AudioCodec, AudioCodecPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Retrieves information about a codec property.

func AudioCodecSetProperty(AudioCodec, AudioCodecPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

Sets the value of a codec property.

