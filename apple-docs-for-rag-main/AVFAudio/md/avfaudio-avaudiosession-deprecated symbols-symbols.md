

- AVFAudio
- AVAudioSession
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Topics

### Activating an audio session

func setActive(Bool, withFlags: Int) throws

Activates or deactivates your app’s audio session; provides flags for use by other audio sessions.

Deprecated

### Requesting permission to record

var recordPermission: AVAudioSession.RecordPermission

The current recording permission status.

Deprecated

func requestRecordPermission((Bool) -> Void)

Requests the user’s permission to record audio.

Deprecated

### Inspecting audio hardware

var currentHardwareInputNumberOfChannels: Int

The number of audio hardware input channels.

Deprecated

var currentHardwareOutputNumberOfChannels: Int

The number of audio hardware output channels.

Deprecated

var currentHardwareSampleRate: Double

The audio hardware sample rate, in hertz.

Deprecated

var inputIsAvailable: Bool

A Boolean value that indicates whether a hardware audio input path is available.

Deprecated

var preferredHardwareSampleRate: Double

The preferred hardware sample rate, in hertz.

Deprecated

func setPreferredHardwareSampleRate(Double) throws

Sets the preferred hardware sample rate for input and output.

Deprecated

### Responding to audio session changes

var delegate: (any AVAudioSessionDelegate)?

The delegate object for the audio session.

Deprecated

protocol AVAudioSessionDelegate

A protocol that defines responses to changes in state for the audio session.

Deprecated

### Handling audio session interruptions

Interruption flags

Constants that indicate the state of the audio session following an interruption.

