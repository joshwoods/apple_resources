

- Audio Toolbox
-  AudioFileTypeAndFormatID 

Structure

# AudioFileTypeAndFormatID

A specifier for the constantkAudioFileGlobalInfo_AvailableStreamDescriptionsForFormat.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioFileTypeAndFormatID
```

## Overview

This structure specifies a desired audio file type and data format ID so you can obtain a list of stream descriptions of available formats.

## Topics

### Initializers

init()

init(mFileType: AudioFileTypeID, mFormatID: UInt32)

### Instance Properties

var mFileType: AudioFileTypeID

A four-character code for the file type.

var mFormatID: UInt32

A four-character code for the format ID such as `kAudioFormatLinearPCM`, `kAudioFormatMPEG4AAC`, and so forth. (See the `AudioFormat.h` header file for declarations.)

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

