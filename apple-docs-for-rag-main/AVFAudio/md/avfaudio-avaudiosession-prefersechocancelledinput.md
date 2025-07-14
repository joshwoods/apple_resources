

- AVFAudio
- AVAudioSession
-  prefersEchoCancelledInput 

Instance Property

# prefersEchoCancelledInput

A Boolean value that indicates the audio session’s preference for using an echo-canceled input.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+

``` source
var prefersEchoCancelledInput: Bool { get }
```

## See Also

### Configuring echo cancellation

var isEchoCancelledInputAvailable: Bool

A Boolean value that indicates whether the built-in microphone and speaker route supports echo cancellation.

var isEchoCancelledInputEnabled: Bool

A Boolean value that indicates whether an echo-canceled input is in an enabled state.

func setPrefersEchoCancelledInput(Bool) throws

Sets a preference to enable echo-canceled input on supported hardware.

