

- AVFAudio
- AVAudioSession
-  isEchoCancelledInputAvailable 

Instance Property

# isEchoCancelledInputAvailable

A Boolean value that indicates whether the built-in microphone and speaker route supports echo cancellation.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.2+

``` source
var isEchoCancelledInputAvailable: Bool { get }
```

## Discussion

This value is `true` if the device supports echo cancellation and the app uses the playAndRecord category and default mode.

## See Also

### Configuring echo cancellation

var isEchoCancelledInputEnabled: Bool

A Boolean value that indicates whether an echo-canceled input is in an enabled state.

func setPrefersEchoCancelledInput(Bool) throws

Sets a preference to enable echo-canceled input on supported hardware.

var prefersEchoCancelledInput: Bool

A Boolean value that indicates the audio session’s preference for using an echo-canceled input.

