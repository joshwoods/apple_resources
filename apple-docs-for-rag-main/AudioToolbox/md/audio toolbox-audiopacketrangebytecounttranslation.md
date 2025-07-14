

- Audio Toolbox
-  AudioPacketRangeByteCountTranslation 

Structure

# AudioPacketRangeByteCountTranslation

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioPacketRangeByteCountTranslation
```

## Topics

### Initializers

init()

init(mPacket: Int64, mPacketCount: Int64, mByteCountUpperBound: Int64)

### Instance Properties

var mByteCountUpperBound: Int64

var mPacket: Int64

var mPacketCount: Int64

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

struct AudioBytePacketTranslation

A data structure used by the kAudioFilePropertyByteToPacket and kAudioFilePropertyPacketToByte properties.

