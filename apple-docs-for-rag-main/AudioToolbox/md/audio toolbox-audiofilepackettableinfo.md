

- Audio Toolbox
-  AudioFilePacketTableInfo 

Structure

# AudioFilePacketTableInfo

Contains information about the number of valid frames in a file and where they begin and end.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioFilePacketTableInfo
```

## Overview

Some data formats might have packets with contents that are not completely valid, but that represent priming or remainder frames not intended for playback. For example, a file with 100 packets of AAC is nominally 1024 \* 100 = 102400 frames of data. However, the first 2112 frames might be priming frames.

A number of remainder frames might be added to pad out to a full packet of 1024 frames. Discard the priming and remainder frames.

The total number of packets in the file times the frames per packet (or counting each packet’s frames individually for a variable frames per packet format) minus `mPrimingFrames`, minus `mRemainderFrames`, should equal `mNumberValidFrames`.

## Topics

### Initializers

init()

init(mNumberValidFrames: Int64, mPrimingFrames: Int32, mRemainderFrames: Int32)

### Instance Properties

var mNumberValidFrames: Int64

The number of valid frames in the file.

var mPrimingFrames: Int32

The number of invalid frames at the beginning of the file.

var mRemainderFrames: Int32

The number of invalid frames at the end of the file.

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

