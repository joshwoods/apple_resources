

- Audio Toolbox
-  AudioConverterNew(\_:\_:\_:) 

Function

# AudioConverterNew(\_:\_:\_:)

Creates a new audio converter object based on specified audio formats.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.1+tvOS 9.0+visionOS 1.0+

``` source
func AudioConverterNew(
    _ inSourceFormat: UnsafePointer,
    _ inDestinationFormat: UnsafePointer,
    _ outAudioConverter: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inSourceFormat`  

The format of the source audio to be converted.

`inDestinationFormat`  

The destination format to which the audio is to be converted.

`outAudioConverter`  

On return, a new audio converter object.

## Return Value

A result code.

## Discussion

For a pair of linear PCM formats, the following conversions are supported:

- Addition and removal of channels, when the input and output format `mChannelsPerFrame` fields do not match. Channels may also be reordered and removed using the `kAudioConverterChannelMap` property.

- Sample rate conversion.

- Interleaving and deinterleaving, when the input and output format `(mFormatFlags & kAudioFormatFlagIsNonInterleaved)` values do not match.

- Conversion between any pair of the following formats:

- 8-bit integer, signed or unsigned.

- 16-, 24-, or 32-bit integer, big- or little-endian. Other integral bit depths, if high-aligned and nonpacked, are also supported

- 32- and 64-bit floating point, big- or little-endian.

Encoding and decoding between linear PCM and compressed formats is supported. Functions in Audio Format Services (`AudioToolbox/AudioFormat.h`) return information about the formats supported on a system. When using a codec, you can use any supported PCM format. The converter object performs any necessary additional conversion between your PCM format and the one created or consumed by the codec.

## See Also

### Managing Audio Converter Objects

func AudioConverterNewSpecific(UnsafePointer&lt;AudioStreamBasicDescription>, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32, UnsafePointer&lt;AudioClassDescription>, UnsafeMutablePointer&lt;AudioConverterRef?>) -> OSStatus

Creates a new audio converter object using a specified codec.

func AudioConverterReset(AudioConverterRef) -> OSStatus

Resets an audio converter object, clearing and flushing its buffers.

func AudioConverterDispose(AudioConverterRef) -> OSStatus

Disposes of an audio converter object.

