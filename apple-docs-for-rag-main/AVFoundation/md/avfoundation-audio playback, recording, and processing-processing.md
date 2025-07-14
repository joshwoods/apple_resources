

- AVFoundation
-  Audio playback, recording, and processing 

API Collection

# Audio playback, recording, and processing

Play, record, and process audio; configure your app’s system audio behavior.

## Topics

### System audio

Handling audio interruptions

Observe audio session notifications to ensure that your app responds appropriately to interruptions.

Responding to audio route changes

Observe audio session notifications to ensure that your app responds appropriately to route changes.

Capturing stereo audio from built-In microphones

Configure an iOS device’s built-in microphones to add stereo recording capabilities to your app.

class AVAudioSession

An object that communicates to the system how you intend to use audio in your app.

protocol AVAudioSessionSpatialExperience

A protocol that defines types of spatial audio experiences that the system supports.

class AVAudioApplication

An object that manages one or more audio sessions that belong to an app.

class AVAudioRoutingArbiter

An object for configuring macOS apps to participate in AirPods Automatic Switching.

### Basic playback and recording

class AVAudioPlayer

An object that plays audio data from a file or buffer.

class AVAudioRecorder

An object that records audio data to a file.

class AVMIDIPlayer

An object that plays MIDI data through a system sound module.

### Advanced audio processing

Audio Engine

Perform advanced real-time and offline audio processing, implement 3D spatialization, and work with MIDI and samplers.

## See Also

### Audio

Speech synthesis

Configure voices to speak strings of text.

