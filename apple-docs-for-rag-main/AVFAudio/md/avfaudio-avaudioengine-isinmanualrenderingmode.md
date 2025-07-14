

- AVFAudio
- AVAudioEngine
-  isInManualRenderingMode 

Instance Property

# isInManualRenderingMode

A Boolean value that indicates whether the engine is operating in manual rendering mode.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var isInManualRenderingMode: Bool { get }
```

## See Also

### Getting Manual Rendering Properties

typealias AVAudioEngineManualRenderingBlock

The type that represents a block that renders the engine when operating in manual rendering mode.

var manualRenderingBlock: AVAudioEngineManualRenderingBlock

The block that renders the engine when operating in manual rendering mode.

var manualRenderingFormat: AVAudioFormat

The render format of the engine in manual rendering mode.

var manualRenderingMaximumFrameCount: AVAudioFrameCount

The maximum number of PCM sample frames the engine produces in any single render call in manual rendering mode.

var manualRenderingMode: AVAudioEngineManualRenderingMode

The manual rendering mode configured on the engine.

var manualRenderingSampleTime: AVAudioFramePosition

An indication of where the engine is on its render timeline in manual rendering mode.

var isAutoShutdownEnabled: Bool

A Boolean value that indicates whether autoshutdown is in an enabled state.

