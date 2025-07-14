

- AVFAudio
- AVAudioSession
-  isMicrophoneInjectionAvailable 

Instance Property

# isMicrophoneInjectionAvailable

A Boolean value that indicates whether microphone injection is available.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.2+

``` source
var isMicrophoneInjectionAvailable: Bool { get }
```

## Discussion

Observe changes to the value of this property by registering for notifications of type microphoneInjectionCapabilitiesChangeNotification.

## See Also

### Enabling adding audio to calls

var preferredMicrophoneInjectionMode: AVAudioSession.MicrophoneInjectionMode

The preferred mode of injecting audio into another app’s input stream.

func setPreferredMicrophoneInjectionMode(AVAudioSession.MicrophoneInjectionMode) throws

Sets the preferred mode of injecting audio into another app’s input stream.

enum MicrophoneInjectionMode

The modes of injecting audio into another app’s input stream.

class let microphoneInjectionCapabilitiesChangeNotification: NSNotification.Name

A notification the system posts when its capability to inject audio into an input stream changes.

