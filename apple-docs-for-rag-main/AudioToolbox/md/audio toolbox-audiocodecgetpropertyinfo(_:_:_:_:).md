

- Audio Toolbox
-  AudioCodecGetPropertyInfo(\_:\_:\_:\_:) 

Function

# AudioCodecGetPropertyInfo(\_:\_:\_:\_:)

Retrieves information about a codec property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func AudioCodecGetPropertyInfo(
    _ inCodec: AudioCodec,
    _ inPropertyID: AudioCodecPropertyID,
    _ outSize: UnsafeMutablePointer?,
    _ outWritable: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`inCodec`  

An audio codec object. Because an audio codec object is a Component Manger component instance, you can use the Component Manager (for example, the functions FindNextComponent and OpenAComponent) to obtain an audio codec object.

`inPropertyID`  

Property ID of the property about which you want to obtain information. Codec property IDs are listed in Global Codec Properties and Instance Codec Properties.

`outSize`  

On return, size in bytes of the current value of the property.

`outWritable`  

Returns `true` if you can change the value of the property, otherwise `false`.

## Return Value

Returns `NoErr` if successful, otherwise, a result code. See `Result Codes` for a list of possible values.

## Discussion

Call this function to:

- get the size of a property value before calling AudioCodecGetProperty(_:_:_:_:) to retrieve the value

- find out if a property value can be modified before calling AudioCodecSetProperty(_:_:_:_:) to set the value

## See Also

### Accessing Codec Properties

func AudioCodecGetProperty(AudioCodec, AudioCodecPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Retrieves the value of a codec property.

func AudioCodecSetProperty(AudioCodec, AudioCodecPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

Sets the value of a codec property.

