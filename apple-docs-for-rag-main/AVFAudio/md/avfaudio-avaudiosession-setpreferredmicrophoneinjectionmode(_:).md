

- AVFAudio
- AVAudioSession
-  setPreferredMicrophoneInjectionMode(\_:) 

Instance Method

# setPreferredMicrophoneInjectionMode(\_:)

Sets the preferred mode of injecting audio into another app’s input stream.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.2+

``` source
func setPreferredMicrophoneInjectionMode(_ inValue: AVAudioSession.MicrophoneInjectionMode) throws
```

## Parameters 

`inValue`  

The preferred microphone injection mode.

## See Also

### Enabling adding audio to calls

var isMicrophoneInjectionAvailable: Bool

A Boolean value that indicates whether microphone injection is available.

var preferredMicrophoneInjectionMode: AVAudioSession.MicrophoneInjectionMode

The preferred mode of injecting audio into another app’s input stream.

enum MicrophoneInjectionMode

The modes of injecting audio into another app’s input stream.

class let microphoneInjectionCapabilitiesChangeNotification: NSNotification.Name

A notification the system posts when its capability to inject audio into an input stream changes.

