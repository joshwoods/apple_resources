

- AVFAudio
- AVAudioSession
-  AVAudioSession.MicrophoneInjectionMode 

Enumeration

# AVAudioSession.MicrophoneInjectionMode

The modes of injecting audio into another app’s input stream.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
enum MicrophoneInjectionMode
```

## Overview

Apps can state their intent to mix synthesized speech into another app’s input stream. Accessibility apps can use this feature to implement augmentative and alternative communication systems that enable people with disabilities to communicate using synthesized speech.

Note

When a person mutes audio input, the system also mutes microphone injection.

## Topics

### Microphone injection modes

case none

A mode that indicates not to use spoken audio injection.

case spokenAudio

A mode that indicates to inject spoken audio, like synthesized speech, along with microphone audio.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enabling adding audio to calls

var isMicrophoneInjectionAvailable: Bool

A Boolean value that indicates whether microphone injection is available.

var preferredMicrophoneInjectionMode: AVAudioSession.MicrophoneInjectionMode

The preferred mode of injecting audio into another app’s input stream.

func setPreferredMicrophoneInjectionMode(AVAudioSession.MicrophoneInjectionMode) throws

Sets the preferred mode of injecting audio into another app’s input stream.

class let microphoneInjectionCapabilitiesChangeNotification: NSNotification.Name

A notification the system posts when its capability to inject audio into an input stream changes.

