

- Audio Toolbox
-  AudioCodecSetProperty(\_:\_:\_:\_:) 

Function

# AudioCodecSetProperty(\_:\_:\_:\_:)

Sets the value of a codec property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func AudioCodecSetProperty(
    _ inCodec: AudioCodec,
    _ inPropertyID: AudioCodecPropertyID,
    _ inPropertyDataSize: UInt32,
    _ inPropertyData: UnsafeRawPointer
) -> OSStatus
```

## Parameters 

`inCodec`  

An audio codec object. Because an audio codec object is a Component Manger component instance, you can use the Component Manager (for example, the functions FindNextComponent and OpenAComponent) to obtain an audio codec object.

`inPropertyID`  

Property ID of the property whose value you want to set. Settable codec property IDs are listed in Instance Codec Properties.

`inPropertyDataSize`  

Size in bytes of the property value data.

`inPropertyData`  

Pointer to the data buffer containing the property value.

## Return Value

Returns `NoErr` if successful, otherwise, a result code. See `Result Codes` for a list of possible values.

## Discussion

Codec properties are classified as either global properties, which remain the same for all instances of a codec, or instance properties, which may vary from instance to instance. However, not all instance property values can be modified. See Instance Codec Properties for details. No property values can be modified when the codec is in the initialized state. You must call this function before you call the AudioCodecInitialize(_:_:_:_:_:) function, or after you call the AudioCodecUninitialize(_:) function. Call the AudioCodecGetProperty(_:_:_:_:) function to retrieve the current value of a property.

## See Also

### Related Documentation

func AudioCodecUninitialize(AudioCodec) -> OSStatus

Moves the codec from the initialized state back to the uninitialized state.

func AudioCodecInitialize(AudioCodec, UnsafePointer&lt;AudioStreamBasicDescription>?, UnsafePointer&lt;AudioStreamBasicDescription>?, UnsafeRawPointer?, UInt32) -> OSStatus

Sets up the specified codec to perform a data format translation.

### Accessing Codec Properties

func AudioCodecGetProperty(AudioCodec, AudioCodecPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Retrieves the value of a codec property.

func AudioCodecGetPropertyInfo(AudioCodec, AudioCodecPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Retrieves information about a codec property.

