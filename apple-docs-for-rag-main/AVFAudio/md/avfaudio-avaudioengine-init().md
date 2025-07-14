

- AVFAudio
- AVAudioEngine
-  init() 

Initializer

# init()

Creates an audio engine instance for rendering in real time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init()
```

## Return Value

A new `AVAudioEngine` instance.

## Discussion

To operate in manual rendering mode, which removes real-time running constraints, see enableManualRenderingMode(_:format:maximumFrameCount:).

