

- Audio Toolbox
-  AudioBytePacketTranslation 

Structure

# AudioBytePacketTranslation

A data structure used by the kAudioFilePropertyByteToPacket and kAudioFilePropertyPacketToByte properties.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioBytePacketTranslation
```

## Topics

### Initializers

init()

init(mByte: Int64, mPacket: Int64, mByteOffsetInPacket: UInt32, mFlags: AudioBytePacketTranslationFlags)

### Instance Properties

var mByte: Int64

A byte number.

var mByteOffsetInPacket: UInt32

A byte offset in a packet.

var mFlags: AudioBytePacketTranslationFlags

A translation flag value.

var mPacket: Int64

A packet number.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

struct AudioBytePacketTranslationFlags

struct AudioFileFlags

struct AudioFileRegionFlags

Flags that specify a playback direction for an audio file region structure.

struct AudioFileStreamParseFlags

struct AudioFileStreamPropertyFlags

struct AudioFileStreamSeekFlags

typealias AudioFileID

An opaque data type that represents an audio file object.

typealias AudioFilePropertyID

An audio file property identifier.

struct AudioFile_SMPTE_Time

A data structure for describing SMPTE (Society of Motion Picture and Television Engineers) time.

struct AudioFileMarker

Annotates a position in an audio file.

struct AudioFileMarkerList

A list of markers associated with an audio file, including their SMPTE time type, the number of markers, and the markers themselves.

struct AudioFileRegion

An audio file region specifies a segment of audio data.

struct AudioFileRegionList

A list of the audio file regions in a file.

struct AudioFramePacketTranslation

A structure that specifies frame and packet translations.

struct AudioFilePacketTableInfo

Contains information about the number of valid frames in a file and where they begin and end.

