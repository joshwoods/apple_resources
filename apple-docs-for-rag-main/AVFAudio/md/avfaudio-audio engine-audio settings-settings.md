

- AVFAudio
- Audio Engine
-  Audio settings 

API Collection

# Audio settings

Configure audio processing settings using standard key and value constants.

## Topics

### Formats

class AVAudioFormat

An object that describes the representation of an audio format.

class AVAudioChannelLayout

An object that describes the roles of a set of audio channels.

let AVChannelLayoutKey: String

Linear PCM Format Settings

The audio settings that apply to linear PCM audio formats.

Format Settings

The audio settings that apply to all audio formats that the audio player and recorder classes support.

### Settings

Sample Rate Conversion Settings

The constants that define sample rate converter audio quality settings.

enum AVAudioQuality

The values that specify the sample rate audio quality for encoding and conversion.

let AVEncoderAudioQualityKey: String

A constant that represents an integer from the audio quality enumeration.

Encoder Settings

The constants that define the audio encoder settings for the audio recorder class.

Time Pitch Algorithm Settings

The constants that define the values for the time pitch algorithms.

### Constants

Encoder Bit Rate Strategy Values

The constants that represent the possible bit rate strategy values.

var AVAUDIOENGINE_HAVE_AUAUDIOUNIT: Int32

## See Also

### Supporting data types

class AVAudioBuffer

An object that represents a buffer of audio data with a format.

class AVAudioFile

An object that represents an audio file that the system can open for reading or writing.

class AVAudioTime

An object you use to represent a moment in time.

