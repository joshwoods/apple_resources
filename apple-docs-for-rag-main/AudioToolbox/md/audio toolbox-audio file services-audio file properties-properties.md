

- Audio Toolbox
- Audio File Services
-  Audio File Properties 

API Collection

# Audio File Properties

Properties used by the functions described in getting and setting pieces of data in audio files. See Working with Global Information for details.

## Topics

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

var kAudioFilePropertyFrameToPacket: AudioFilePropertyID

Passes an audio frame packet translation structure with the `mFrame` field filled out and returns the `mPacket` and `mFrameOffsetInPacket` fields.

var kAudioFilePropertyPacketToByte: AudioFilePropertyID

Passes an audio byte packet translation structure with the `mPacket` field filled out and returns the `mByte` field. The `mByteOffsetInPacket` field is ignored. If the value in the `mByte` field is an estimate then the `kBytePacketTranslationFlag_IsEstimate` flag is set in the `mFlags` field.

var kAudioFilePropertyByteToPacket: AudioFilePropertyID

Passes an audio byte packet translation structure with the `mByte` field filled out and returns the `mPacket` and `mByteOffsetInPacket` fields. If the value in the `mByte` field is an estimate then the `kBytePacketTranslationFlag_IsEstimate` flag is set in the `mFlags` field.

var kAudioFilePropertyChunkIDs: AudioFilePropertyID

An array of four-character codes for each kind of chunk in the file.

var kAudioFilePropertyInfoDictionary: AudioFilePropertyID

A CF Dictionary with information about the data in the file.

var kAudioFilePropertyPacketTableInfo: AudioFilePropertyID

Gets or sets an audio file packet table information structure for its supporting file types. When setting the structure, the sum of the values of the `mNumberValidFrames`, `mPrimingFrames` and `mRemainderFrames` fields must be the same as the total number of frames in all packets. If not, a `paramErr` is returned. To ensure this result, get the value of the property and make sure the sum of the three values you set has the same sum as the three values you got.

var kAudioFilePropertyPacketSizeUpperBound: AudioFilePropertyID

The theoretical maximum packet size in the file. This value is obtained without actually scanning the whole file to find the largest packet, as could happen with `kAudioFilePropertyMaximumPacketSize`.

var kAudioFilePropertyReserveDuration: AudioFilePropertyID

The duration in seconds of the data expected to be written. Set this property before any data has been written to reserve space in the file header for a packet table and other information to appear before the audio data. Otherwise, the packet table might get written at the end of the file, preventing the file from being streamable.

var kAudioFilePropertyEstimatedDuration: AudioFilePropertyID

An estimated duration in seconds. If this duration can be calculated without scanning the entire file, or all the audio data packets have been scanned, the value accurately reflects the duration of the audio data.

var kAudioFilePropertyBitRate: AudioFilePropertyID

The actual bit rate (number of audio data bits in the file divided by the duration of the file) for some file types, and the nominal bit rate (which bit rate the encoder was set to) for others.

var kAudioFilePropertyID3Tag: AudioFilePropertyID

A `void*` value pointing to memory set up by your application to contain a fully formatted ID3 tag.

var kAudioFilePropertySourceBitDepth: AudioFilePropertyID

For compressed data, this property’s value is the bit depth of the source, uncompressed audio stream as an `SInt32` value, if known. The bit depth is expressed as a negative number if the uncompressed source was in a floating point format. For example, a property value of `-32` is used for `float` and a property value of `-64` represents `double`.

var kAudioFilePropertyAlbumArtwork: AudioFilePropertyID

An object containing the image data for the album artwork associated with an audio file.

var kAudioFilePropertyAudioTrackCount: AudioFilePropertyID

var kAudioFilePropertyUseAudioTrack: AudioFilePropertyID

var kAudioFilePropertyID3TagOffset: AudioFilePropertyID

var kAudioFilePropertyNextIndependentPacket: AudioFilePropertyID

var kAudioFilePropertyPacketRangeByteCountUpperBound: AudioFilePropertyID

var kAudioFilePropertyPacketToDependencyInfo: AudioFilePropertyID

var kAudioFilePropertyPacketToRollDistance: AudioFilePropertyID

var kAudioFilePropertyPreviousIndependentPacket: AudioFilePropertyID

var kAudioFilePropertyRestrictsRandomAccess: AudioFilePropertyID

## See Also

### Constants

typealias AudioFileTypeID

Operating system constants that indicate the type of file to be written or a hint about what type of file to expect from data provided.

Audio File Creation Flags

Flags to set when creating an audio file.

enum AudioFilePermissions

Flags for use when opening an audio file.

Audio File Loop Direction Constants

The playback direction of a looped segment of an audio file.

Audio File Marker Types

A type of marker within a file used in the `mType` field of the AudioFileMarker structure.

struct AudioFileRegionFlags

Flags that specify a playback direction for an audio file region structure.

Audio File Packet Translation Flags

Flags specified in a packet translation structure.

Info String Keys

Key values of properties to get and set using Audio File Services functions and provide a common way to get the same information out of several different kinds of files.

Audio File Global Info Properties

Access these properties using the functions described in Working with Global Information.

