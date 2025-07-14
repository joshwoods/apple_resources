

- Audio Toolbox
-  AudioFileFlags 

Structure

# AudioFileFlags

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioFileFlags
```

## Topics

### Flags

static var dontPageAlignAudioData: AudioFileFlags

Typically, the audio data in a file is page aligned. To make reading the file data as fast as possible, you can use page-aligned data to take advantage of optimized code paths in the file system. However, when space is at a premium, you might want to avoid the additional padding required to attain alignment. To do so, set this flag when calling AudioFileCreate or AudioFileCreateWithURL(_:_:_:_:_:).

static var eraseFile: AudioFileFlags

### Initializers

init(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Data Types

struct AudioBytePacketTranslationFlags

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

struct AudioFilePacketTableInfo

Contains information about the number of valid frames in a file and where they begin and end.

