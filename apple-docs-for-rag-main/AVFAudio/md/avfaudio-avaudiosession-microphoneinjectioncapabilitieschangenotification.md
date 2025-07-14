

- AVFAudio
- AVAudioSession
-  microphoneInjectionCapabilitiesChangeNotification 

Type Property

# microphoneInjectionCapabilitiesChangeNotification

A notification the system posts when its capability to inject audio into an input stream changes.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.2+

``` source
class let microphoneInjectionCapabilitiesChangeNotification: NSNotification.Name
```

## Discussion

Query the notification’s `userInfo` dictionary for AVAudioSessionMicrophoneInjectionIsAvailableKey to determine whether microphone injection is available.

## Topics

### User-information keys

let AVAudioSessionMicrophoneInjectionIsAvailableKey: String

A key to retrieve a Boolean value that indicates whether microphone injection is available.

## See Also

### Enabling adding audio to calls

var isMicrophoneInjectionAvailable: Bool

A Boolean value that indicates whether microphone injection is available.

var preferredMicrophoneInjectionMode: AVAudioSession.MicrophoneInjectionMode

The preferred mode of injecting audio into another app’s input stream.

func setPreferredMicrophoneInjectionMode(AVAudioSession.MicrophoneInjectionMode) throws

Sets the preferred mode of injecting audio into another app’s input stream.

enum MicrophoneInjectionMode

The modes of injecting audio into another app’s input stream.

