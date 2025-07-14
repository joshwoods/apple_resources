

- RealityKit
- AudioBufferResource
-  init(buffer:configuration:) 

Initializer

# init(buffer:configuration:)

Creates an `AudioBufferResource` with the given `AVAudioBuffer` and configuration.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
init(
    buffer: AVAudioBuffer,
    configuration: AudioBufferResource.Configuration = .init()
) throws
```

## Discussion

Throws

An error if the given `buffer` is not or cannot be converted to a non-interleaved PCM buffer.

