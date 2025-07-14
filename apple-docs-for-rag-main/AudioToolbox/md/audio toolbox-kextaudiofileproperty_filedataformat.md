

- Audio Toolbox
-  kExtAudioFileProperty_FileDataFormat 

Global Variable

# kExtAudioFileProperty_FileDataFormat

A file’s data format.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kExtAudioFileProperty_FileDataFormat: ExtAudioFilePropertyID { get }
```

## Discussion

A file’s data format. Value is a read-only AudioStreamBasicDescription struct.

## See Also

### Constants

var kExtAudioFileProperty_FileChannelLayout: ExtAudioFilePropertyID

A file’s channel layout.

var kExtAudioFileProperty_ClientDataFormat: ExtAudioFilePropertyID

The audio stream format for your application.

var kExtAudioFileProperty_ClientChannelLayout: ExtAudioFilePropertyID

The audio channel layout for your application.

var kExtAudioFileProperty_CodecManufacturer: ExtAudioFilePropertyID

The manufacturer of the codec to be used by the extended audio file object. Value is a read/write `UInt32`.

var kExtAudioFileProperty_AudioConverter: ExtAudioFilePropertyID

The audio converter object associated with the extended audio file object, if a converter is associated.

var kExtAudioFileProperty_AudioFile: ExtAudioFilePropertyID

The audio file object associated with the extended audio file object.

var kExtAudioFileProperty_FileMaxPacketSize: ExtAudioFilePropertyID

The file data format’s maximum packet size, in bytes. Value is a read-only `UInt32`.

var kExtAudioFileProperty_ClientMaxPacketSize: ExtAudioFilePropertyID

Your application audio data format’s maximum packet size, in bytes. Value is a read-only `UInt32`.

var kExtAudioFileProperty_FileLengthFrames: ExtAudioFilePropertyID

The associated audio file’s length in sample frames. Value is an `SInt64`. For a PCM file, the value is read/write. For a non-PCM file, the value is read-only.

var kExtAudioFileProperty_ConverterConfig: ExtAudioFilePropertyID

The configuration of the extended audio file object’s associated audio converter, as specified by the `kAudioConverterPropertySettings` property. Value is a read/write `CFArray` object.

var kExtAudioFileProperty_IOBufferSizeBytes: ExtAudioFilePropertyID

The size of the buffer that the extended audio file object’s associated audio converter uses to read or write the associated audio file. Value is a read/write `UInt32`.

var kExtAudioFileProperty_IOBuffer: ExtAudioFilePropertyID

An audio data buffer. Value is a read/write `void*` value.

var kExtAudioFileProperty_PacketTable: ExtAudioFilePropertyID

This property can be used to override the priming and remainder information in an audio file, and also to retrieve the current priming and remainder frames information for an extended audio file object. If the underlying file type does not provide packet table information, attempting to get the value of this property returns an error.

