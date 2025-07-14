

- Audio Toolbox
-  AudioFile_SMPTE_Time 

Structure

# AudioFile_SMPTE_Time

A data structure for describing SMPTE (Society of Motion Picture and Television Engineers) time.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioFile_SMPTE_Time
```

## Topics

### Initializers

init()

init(mHours: Int8, mMinutes: UInt8, mSeconds: UInt8, mFrames: UInt8, mSubFrameSampleOffset: UInt32)

### Instance Properties

var mFrames: UInt8

The frames.

var mHours: Int8

The hours.

var mMinutes: UInt8

The minutes.

var mSeconds: UInt8

The seconds.

var mSubFrameSampleOffset: UInt32

The sample offset within a frame.

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

struct AudioBytePacketTranslation

A data structure used by the kAudioFilePropertyByteToPacket and kAudioFilePropertyPacketToByte properties.

struct AudioFilePacketTableInfo

Contains information about the number of valid frames in a file and where they begin and end.

