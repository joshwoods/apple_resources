

- AVFAudio
- AVAudioSession
-  isEchoCancelledInputEnabled 

Instance Property

# isEchoCancelledInputEnabled

A Boolean value that indicates whether an echo-canceled input is in an enabled state.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+

``` source
var isEchoCancelledInputEnabled: Bool { get }
```

## Discussion

For more information about echo cancellation, see setPrefersEchoCancelledInput(_:).

## See Also

### Configuring echo cancellation

var isEchoCancelledInputAvailable: Bool

A Boolean value that indicates whether the built-in microphone and speaker route supports echo cancellation.

func setPrefersEchoCancelledInput(Bool) throws

Sets a preference to enable echo-canceled input on supported hardware.

var prefersEchoCancelledInput: Bool

A Boolean value that indicates the audio session’s preference for using an echo-canceled input.

