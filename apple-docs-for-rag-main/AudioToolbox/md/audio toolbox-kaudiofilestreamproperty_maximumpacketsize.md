

- Audio Toolbox
-  kAudioFileStreamProperty_MaximumPacketSize 

Global Variable

# kAudioFileStreamProperty_MaximumPacketSize

A `UInt32` value indicating the maximum packet size of the data in the streamed file.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioFileStreamProperty_MaximumPacketSize: AudioFileStreamPropertyID { get }
```

## See Also

### Constants

var kAudioFileStreamProperty_ReadyToProducePackets: AudioFileStreamPropertyID

var kAudioFileStreamProperty_FileFormat: AudioFileStreamPropertyID

A four-character code that identifies the audio data format.

var kAudioFileStreamProperty_DataFormat: AudioFileStreamPropertyID

An `AudioStreamBasicDescription` structure describing the format of the audio data in the stream.

var kAudioFileStreamProperty_FormatList: AudioFileStreamPropertyID

To support formats such as AAC with SBR where an encoded data stream can be decoded to multiple destination formats, this property returns an array of `AudioFormatListItem` structures (declared in `AudioFormat.h`)—one for each of the destination formats. The default behavior is to return an `AudioFormatListItem` structure that has the same `AudioStreamBasicDescription` structure as that returned by the kAudioFileStreamProperty_DataFormat property.

var kAudioFileStreamProperty_MagicCookieData: AudioFileStreamPropertyID

A pointer (`void *`) to a magic cookie. For audio file types that require a magic cookie before packets can be written to a file, you should get this property value before calling the AudioFileWriteBytes(_:_:_:_:_:) or AudioFileWritePackets(_:_:_:_:_:_:_:) functions.

var kAudioFileStreamProperty_AudioDataByteCount: AudioFileStreamPropertyID

A `UInt64` value indicating the number of bytes of audio data in the streamed file. This property is valid only if the number of bytes for the entire stream is known from the data parsed in the header. For some kinds of streams this property may have no value.

var kAudioFileStreamProperty_AudioDataPacketCount: AudioFileStreamPropertyID

A `UInt64` value indicating the number of packets of audio data in the streamed file.

var kAudioFileStreamProperty_DataOffset: AudioFileStreamPropertyID

An `SInt64` value indicating the byte offset in the streamed file at which the audio data starts.

var kAudioFileStreamProperty_ChannelLayout: AudioFileStreamPropertyID

An `AudioChannelLayout` structure.

var kAudioFileStreamProperty_PacketToFrame: AudioFileStreamPropertyID

Obtains the frame number corresponding to a packet number.

var kAudioFileStreamProperty_FrameToPacket: AudioFileStreamPropertyID

Obtains the packet number corresponding to a frame number.

var kAudioFileStreamProperty_PacketToByte: AudioFileStreamPropertyID

Obtains the byte number corresponding to a packet number. Pass an `AudioBytePacketTranslation` structure with the `mPacket` field filled in, and a value is returned in the `mByte` field. The `mByteOffsetInPacket` field of the `AudioBytePacketTranslation` structure is ignored. If the `mByte` value is an estimate, then the `kBytePacketTranslationFlag_IsEstimate` value will be set in the `mFlags` field.

var kAudioFileStreamProperty_ByteToPacket: AudioFileStreamPropertyID

Obtains the packet number corresponding to a byte number. Pass an `AudioBytePacketTranslation` structure with the `mByte` field filled in, and values are returned in the `mPacket` and `mByteOffsetInPacket` fields. If the `mPacket` value is an estimate, then the `kBytePacketTranslationFlag_IsEstimate` value will be set in the `mFlags` field.

var kAudioFileStreamProperty_PacketTableInfo: AudioFileStreamPropertyID

An `AudioFilePacketTableInfo` structure.

var kAudioFileStreamProperty_PacketSizeUpperBound: AudioFileStreamPropertyID

A `UInt32` value indicating the theoretical maximum packet size in the streamed file. This value is useful for determining minimum buffer sizes, for example.

