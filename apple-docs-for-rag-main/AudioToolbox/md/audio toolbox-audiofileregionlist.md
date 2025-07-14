

- Audio Toolbox
-  AudioFileRegionList 

Structure

# AudioFileRegionList

A list of the audio file regions in a file.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioFileRegionList
```

## Overview

This structure is used by the kAudioFilePropertyRegionList property.

## Topics

### Initializers

init()

init(mSMPTE_TimeType: UInt32, mNumberRegions: UInt32, mRegions: AudioFileRegion)

### Instance Properties

var mNumberRegions: UInt32

The number of regions in the list specified in the `mRegions` parameter.

var mRegions: AudioFileRegion

A variable length array of audio file regions.

var mSMPTE_TimeType: UInt32

The SMPTE timing scheme used in the file. See Core Audio’s `CAFFile.h` header file for the values used here. For more information, see *Core Audio Overview*.

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

struct AudioFileMarkerList

A list of markers associated with an audio file, including their SMPTE time type, the number of markers, and the markers themselves.

struct AudioFileRegion

An audio file region specifies a segment of audio data.

struct AudioFramePacketTranslation

A structure that specifies frame and packet translations.

struct AudioBytePacketTranslation

A data structure used by the kAudioFilePropertyByteToPacket and kAudioFilePropertyPacketToByte properties.

struct AudioFilePacketTableInfo

Contains information about the number of valid frames in a file and where they begin and end.

