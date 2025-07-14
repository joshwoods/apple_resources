

- Audio Toolbox
- Audio File Services
-  Audio File Loop Direction Constants 

API Collection

# Audio File Loop Direction Constants

The playback direction of a looped segment of an audio file.

## Topics

### Constants

var kAudioFileLoopDirection_NoLooping: UInt32

The segment is not looped.

var kAudioFileLoopDirection_Forward: UInt32

Play the segment forward.

var kAudioFileLoopDirection_Backward: UInt32

Play the segment backward.

var kAudioFileLoopDirection_ForwardAndBackward: UInt32

Play the segment forward and backward.

## See Also

### Constants

typealias AudioFileTypeID

Operating system constants that indicate the type of file to be written or a hint about what type of file to expect from data provided.

Audio File Creation Flags

Flags to set when creating an audio file.

enum AudioFilePermissions

Flags for use when opening an audio file.

Audio File Marker Types

A type of marker within a file used in the `mType` field of the AudioFileMarker structure.

struct AudioFileRegionFlags

Flags that specify a playback direction for an audio file region structure.

Audio File Packet Translation Flags

Flags specified in a packet translation structure.

Info String Keys

Key values of properties to get and set using Audio File Services functions and provide a common way to get the same information out of several different kinds of files.

Audio File Properties

Properties used by the functions described in getting and setting pieces of data in audio files. See Working with Global Information for details.

Audio File Global Info Properties

Access these properties using the functions described in Working with Global Information.

