

- Audio Toolbox
-  AudioFileRegion 

Structure

# AudioFileRegion

An audio file region specifies a segment of audio data.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioFileRegion
```

## Overview

Typically, a region consists of at least two markers designating the beginning and end of the segment. Other markers might define additional meta information such as sync point.

## Topics

### Initializers

init(mRegionID: UInt32, mName: Unmanaged&lt;CFString>, mFlags: AudioFileRegionFlags, mNumberMarkers: UInt32, mMarkers: AudioFileMarker)

### Instance Properties

var mFlags: AudioFileRegionFlags

Audio File Services region flags.

var mMarkers: AudioFileMarker

An array of `mNumberMarkers` elements describing where the data in the region starts.

var mName: Unmanaged&lt;CFString>

The name of the region.

var mNumberMarkers: UInt32

The number of markers in the array specified in the `mMarkers` parameter.

var mRegionID: UInt32

A unique ID associated with the audio file region.

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

struct AudioFileRegionList

A list of the audio file regions in a file.

struct AudioFramePacketTranslation

A structure that specifies frame and packet translations.

struct AudioBytePacketTranslation

A data structure used by the kAudioFilePropertyByteToPacket and kAudioFilePropertyPacketToByte properties.

struct AudioFilePacketTableInfo

Contains information about the number of valid frames in a file and where they begin and end.

