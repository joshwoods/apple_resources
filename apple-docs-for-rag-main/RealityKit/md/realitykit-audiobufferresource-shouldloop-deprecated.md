

- RealityKit
- AudioBufferResource
-  shouldLoop Deprecated

Instance Property

# shouldLoop

Whether or not this file loops during playback. This should be set for assets that are prepared as seamless loops. A looping resource will play forever until it is explicitly told to stop.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor @preconcurrency
var shouldLoop: Bool { get }
```

Deprecated

Use AudioBufferResource.init(buffer:configuration:) instead.

## See Also

### Deprecated

init(buffer: AVAudioBuffer, inputMode: AudioResource.InputMode, shouldLoop: Bool) throws

Init an AudioBufferResource from an `AVAudioBuffer` instead of a file location. This is intended for use with `AVSpeechSynthesisVoice`.

Deprecated

