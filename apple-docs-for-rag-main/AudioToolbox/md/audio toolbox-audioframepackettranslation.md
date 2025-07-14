

- Audio Toolbox
-  AudioFramePacketTranslation 

Structure

# AudioFramePacketTranslation

A structure that specifies frame and packet translations.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioFramePacketTranslation
```

## Overview

A data structure used by the kAudioFilePropertyPacketToFrame and kAudioFilePropertyFrameToPacket properties.

## Topics

### Initializers

init()

init(mFrame: Int64, mPacket: Int64, mFrameOffsetInPacket: UInt32)

### Instance Properties

var mFrame: Int64

A frame number.

var mFrameOffsetInPacket: UInt32

A frame offset in a packet.

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

struct AudioBytePacketTranslation

A data structure used by the kAudioFilePropertyByteToPacket and kAudioFilePropertyPacketToByte properties.

struct AudioFilePacketTableInfo

Contains information about the number of valid frames in a file and where they begin and end.

