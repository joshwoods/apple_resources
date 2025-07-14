

- Audio Toolbox
-  AudioFileRegionFlags 

Structure

# AudioFileRegionFlags

Flags that specify a playback direction for an audio file region structure.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioFileRegionFlags
```

## Overview

You can set one or more of these flags. For example, if both `kAudioFileRegionFlag_LoopEnable` and `kAudioFileRegionFlag_PlayForward` are set, the region plays as a forward loop. If only `kAudioFileRegionFlag_PlayForward` is set, the region is played forward once. if both `kAudioFileRegionFlag_PlayForward` and `kAudioFileRegionFlag_PlayBackward` are set, the region plays forward then backward, then forward.

## Topics

### Constants

static var loopEnable: AudioFileRegionFlags

If set, the region is looped. You must set one or both of the remaining flags must also be set for the region to be looped.

static var playBackward: AudioFileRegionFlags

If set, the region is played backward.

static var playForward: AudioFileRegionFlags

If set, the region is played forward.

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

struct AudioFileFlags

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

