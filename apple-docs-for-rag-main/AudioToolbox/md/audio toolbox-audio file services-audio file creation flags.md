

- Audio Toolbox
- Audio File Services
-  Audio File Creation Flags 

API Collection

# Audio File Creation Flags

Flags to set when creating an audio file.

## Overview

Flags for use with the AudioFileCreateWithURL(_:_:_:_:_:) and AudioFileCreate functions.

## Topics

### Constants

static var eraseFile: AudioFileFlags

static var dontPageAlignAudioData: AudioFileFlags

Typically, the audio data in a file is page aligned. To make reading the file data as fast as possible, you can use page-aligned data to take advantage of optimized code paths in the file system. However, when space is at a premium, you might want to avoid the additional padding required to attain alignment. To do so, set this flag when calling AudioFileCreate or AudioFileCreateWithURL(_:_:_:_:_:).

## See Also

### Constants

typealias AudioFileTypeID

Operating system constants that indicate the type of file to be written or a hint about what type of file to expect from data provided.

enum AudioFilePermissions

Flags for use when opening an audio file.

Audio File Loop Direction Constants

The playback direction of a looped segment of an audio file.

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

