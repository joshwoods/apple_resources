

- AVFAudio
- AVAudioEngineManualRenderingMode
-  AVAudioEngineManualRenderingMode.realtime 

Case

# AVAudioEngineManualRenderingMode.realtime

An engine that operates under real-time constraints and doesn’t make blocking calls while rendering.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
case realtime
```

## Discussion

You can only use the block-based render mechanism in this mode. See manualRenderingBlock.

## See Also

### Constants

case offline

An engine that operates in an offline mode.

