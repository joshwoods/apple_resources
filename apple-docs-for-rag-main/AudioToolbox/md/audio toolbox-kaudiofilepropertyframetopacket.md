

- Audio Toolbox
-  kAudioFilePropertyFrameToPacket 

Global Variable

# kAudioFilePropertyFrameToPacket

Passes an audio frame packet translation structure with the `mFrame` field filled out and returns the `mPacket` and `mFrameOffsetInPacket` fields.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioFilePropertyFrameToPacket: AudioFilePropertyID { get }
```

## See Also

### Constants

var kAudioFilePropertyFileFormat: AudioFilePropertyID

The format of the audio data file.

var kAudioFilePropertyDataFormat: AudioFilePropertyID

An audio stream basic description containing the format of the audio data.

var kAudioFilePropertyFormatList: AudioFilePropertyID

To support formats such as AAC SBR in which an encoded data stream can be decoded to multiple destination formats, this property’s value is an array of audio format list item values (declared in `AudioFormat.h`) of those formats. Typically, this is an audio format list item with the same audio stream basic description in the `kAudioFilePropertyDataFormat` property.

var kAudioFilePropertyIsOptimized: AudioFilePropertyID

Indicates whether a designated audio file has been optimized, that is, ready to start having sound data written to it. A value of `0` indicates the file needs to be optimized. A value of `1` indicates the file is currently optimized.

var kAudioFilePropertyMagicCookieData: AudioFilePropertyID

A pointer to memory set up by the caller. Some file types require that a magic cookie be provided before packets can be written to an audio file. Set this property before you call AudioFileWriteBytes(_:_:_:_:_:) or AudioFileWritePackets(_:_:_:_:_:_:_:) if a magic cookie exists.

var kAudioFilePropertyAudioDataByteCount: AudioFilePropertyID

Indicates the number of bytes of audio data in the designated file.

var kAudioFilePropertyAudioDataPacketCount: AudioFilePropertyID

Indicates the number of packets of audio data in the designated file.

var kAudioFilePropertyMaximumPacketSize: AudioFilePropertyID

Indicates the maximum size of a packet for the data in the designated file.

var kAudioFilePropertyDataOffset: AudioFilePropertyID

Indicates the byte offset in the file of the designated audio data.

var kAudioFilePropertyChannelLayout: AudioFilePropertyID

An audio channel layout structure.

var kAudioFilePropertyDeferSizeUpdates: AudioFilePropertyID

The default value (`0`) always updates header. If set to `1`, updating the files sizes in the header is not performed every time data is written. Instead, the updating is deferred until the file has been read, optimized, or closed. This process is more efficient, but not as safe. If an application crashes before the size has been updated, the file might not be readable.

var kAudioFilePropertyDataFormatName: AudioFilePropertyID

This constant is deprecated in macOS 10.5 and later. Do not use. Instead, use `kAudioFormatProperty_FormatName` (declared in the `AudioFormat.h` header file).

var kAudioFilePropertyMarkerList: AudioFilePropertyID

A list of audio file markers defined in the file.

var kAudioFilePropertyRegionList: AudioFilePropertyID

The list of audio file region values defined in the file.

var kAudioFilePropertyPacketToFrame: AudioFilePropertyID

Passes an audio frame packet translation structure with the `mPacket` field filled out and returns the `mFrame` field. The `mFrameOffsetInPacket` field is ignored.

