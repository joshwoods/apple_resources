

- Audio Toolbox
-  Audio Unit Voice I/O 

API Collection

# Audio Unit Voice I/O

Configure system voice processing and respond to speech events.

## Topics

### Observing muted speech

var kAUVoiceIOProperty_MutedSpeechActivityEventListener: AudioUnitPropertyID

A property to register a listener that the system calls when it detects speech while the user has the microphone muted.

typealias AUVoiceIOMutedSpeechActivityEventListener

A block that the system calls to indicate speech activity while the user has the microphone muted.

enum AUVoiceIOSpeechActivityEvent

Constants that indicate the state of muted speech.

### Configuring voice processing

var kAUVoiceIOProperty_BypassVoiceProcessing: AudioUnitPropertyID

A property that bypasses all processing for microphone uplink done by the voice processing unit.

var kAUVoiceIOProperty_VoiceProcessingEnableAGC: AudioUnitPropertyID

A property to enable automatic gain control on the processed microphone uplink.

var kAUVoiceIOProperty_MuteOutput: AudioUnitPropertyID

A property to mute the output of the processed microphone uplink.

### Configuring ducking of other audio

struct AUVoiceIOOtherAudioDuckingConfiguration

A structure that you use to configure ducking of other non-voice audio in a voice chat.

### Inspecting errors

var kAUVoiceIOErr_UnexpectedNumberOfInputChannels: OSStatus

An error that indicates that the audio unit encountered an unexpected number of input channels during initialization.

## See Also

### Audio Units

Generating spatial audio from a multichannel audio stream

Convert 8-channel audio to 2-channel spatial audio by using a spatial mixer audio unit.

Audio Unit v3 Plug-Ins

Deliver custom audio effects, instruments, and other audio behaviors using an Audio Unit v3 app extension.

Audio Components

Find, load, and configure audio components, such as Audio Units and audio codecs.

Audio Unit v2 (C) API

Configure an Audio Unit and prepare it to render audio.

Audio Unit Properties

Obtain information about the built-in mixers, equalizers, filters, effects, and other Audio Unit app extensions.

