

- Audio Toolbox
-  kExtAudioFileProperty_AudioConverter 

Global Variable

# kExtAudioFileProperty_AudioConverter

The audio converter object associated with the extended audio file object, if a converter is associated.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kExtAudioFileProperty_AudioConverter: ExtAudioFilePropertyID { get }
```

## Discussion

The value is a read-only AudioConverterRef object.

## Discussion

If you alter any properties of the converter—the bit rate, for instance—you must then set the `kExtAudioFileProperty_ConverterConfig` property. When you do so, using a `NULL` configuration is sufficient. Setting that property ensure that the output file’s data format is consistent with the format being produced by the converter.

## See Also

### Constants

var kExtAudioFileProperty_FileDataFormat: ExtAudioFilePropertyID

A file’s data format.

var kExtAudioFileProperty_FileChannelLayout: ExtAudioFilePropertyID

A file’s channel layout.

var kExtAudioFileProperty_ClientDataFormat: ExtAudioFilePropertyID

The audio stream format for your application.

var kExtAudioFileProperty_ClientChannelLayout: ExtAudioFilePropertyID

The audio channel layout for your application.

var kExtAudioFileProperty_CodecManufacturer: ExtAudioFilePropertyID

The manufacturer of the codec to be used by the extended audio file object. Value is a read/write `UInt32`.

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

