

- Audio Toolbox
-  AudioFileMarkerList 

Structure

# AudioFileMarkerList

A list of markers associated with an audio file, including their SMPTE time type, the number of markers, and the markers themselves.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioFileMarkerList
```

## Topics

### Initializers

init()

init(mSMPTE_TimeType: UInt32, mNumberMarkers: UInt32, mMarkers: AudioFileMarker)

### Instance Properties

var mMarkers: AudioFileMarker

An array of `mNumberMarkers` elements, each of which is an audio file marker.

var mNumberMarkers: UInt32

The number of markers in the list.

var mSMPTE_TimeType: UInt32

The SMPTE time type of the whole list of markers in an audio file.

## Relationships

### Conforms To

- BitwiseCopyable

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

