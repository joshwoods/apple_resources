

- RealityKit
- AudioBufferResource
-  init(buffer:inputMode:shouldLoop:) Deprecated

Initializer

# init(buffer:inputMode:shouldLoop:)

Init an AudioBufferResource from an `AVAudioBuffer` instead of a file location. This is intended for use with `AVSpeechSynthesisVoice`.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0Deprecated

``` source
@MainActor @preconcurrency
init(
    buffer: AVAudioBuffer,
    inputMode: AudioResource.InputMode = .spatial,
    shouldLoop: Bool = false
) throws
```

Deprecated

Use AudioBufferResource.init(buffer:configuration:) instead.

## Parameters 

`inputMode`  

How the audio engine processes a resource. nonSpatial, spatial, ambient

`shouldLoop`  

Bool value to decide if the audio clip should loop

## Discussion

Throws

This function throws an error when the `AVAudioBuffer` cannot be cast or converted to `AVAudioPCMBuffer`.

## See Also

### Deprecated

var shouldLoop: Bool

Whether or not this file loops during playback. This should be set for assets that are prepared as seamless loops. A looping resource will play forever until it is explicitly told to stop.

Deprecated

