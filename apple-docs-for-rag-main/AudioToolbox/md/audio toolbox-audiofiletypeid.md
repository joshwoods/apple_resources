

- Audio Toolbox
-  AudioFileTypeID 

Type Alias

# AudioFileTypeID

Operating system constants that indicate the type of file to be written or a hint about what type of file to expect from data provided.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioFileTypeID = UInt32
```

## Topics

### Constants

var kAudioFileAIFFType: AudioFileTypeID

An Audio Interchange File Format (AIFF) file.

var kAudioFileAIFCType: AudioFileTypeID

An Audio Interchange File Format Compressed (AIFF-C) file.

var kAudioFileWAVEType: AudioFileTypeID

A Microsoft WAVE file.

var kAudioFileSoundDesigner2Type: AudioFileTypeID

A Sound Designer II file.

var kAudioFileNextType: AudioFileTypeID

A NeXT or Sun Microsystems file.

var kAudioFileMP3Type: AudioFileTypeID

An MPEG Audio Layer 3 (`.mp3`) file.

var kAudioFileMP2Type: AudioFileTypeID

An MPEG Audio Layer 2 (`.mp2`) file.

var kAudioFileMP1Type: AudioFileTypeID

An MPEG Audio Layer 1 (`.mp1`) file.

var kAudioFileAC3Type: AudioFileTypeID

An AC-3 file.

var kAudioFileAAC_ADTSType: AudioFileTypeID

An Advanced Audio Coding (AAC) Audio Data Transport Stream (ADTS) file.

var kAudioFileMPEG4Type: AudioFileTypeID

An MPEG 4 file.

var kAudioFileM4AType: AudioFileTypeID

An M4A file.

var kAudioFileCAFType: AudioFileTypeID

A Core Audio File Format file.

var kAudioFile3GPType: AudioFileTypeID

A 3GPP file, suitable for video content on GSM mobile phones.

var kAudioFile3GP2Type: AudioFileTypeID

A 3GPP2 file, suitable for video content on CDMA mobile phones.

var kAudioFileAMRType: AudioFileTypeID

An AMR (Adaptive Multi-Rate) file suitable for compressed speech.

## See Also

### Constants

Audio File Creation Flags

Flags to set when creating an audio file.

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

