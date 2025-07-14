

- Audio Toolbox
-  AudioFileMarker 

Structure

# AudioFileMarker

Annotates a position in an audio file.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioFileMarker
```

## Topics

### Initializers

init()

init(mFramePosition: Float64, mName: Unmanaged&lt;CFString>?, mMarkerID: Int32, mSMPTETime: AudioFile_SMPTE_Time, mType: UInt32, mReserved: UInt16, mChannel: UInt16)

### Instance Properties

var mChannel: UInt16

The channel number referred to by the marker. Set to `0` if the marker applies to all channels.

var mFramePosition: Float64

The frame in the file, counting from the start of the audio data.

var mMarkerID: Int32

A unique ID for the marker.

var mName: Unmanaged&lt;CFString>?

The name of the marker.

var mReserved: UInt16

A reserved field. Set to `0`.

var mSMPTETime: AudioFile_SMPTE_Time

The SMPTE time for this marker.

var mType: UInt32

The marker type.

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

