

- AVFAudio
- AVAudioEngineManualRenderingStatus
-  AVAudioEngineManualRenderingStatus.insufficientDataFromInputNode 

Case

# AVAudioEngineManualRenderingStatus.insufficientDataFromInputNode

A condition that occurs when the input node doesn’t return enough input data to satisfy the render request at the time of the request.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
case insufficientDataFromInputNode
```

## Discussion

This status only applies to the input node when it provides input data for rendering. The output buffer may contain rendered data from other active sources in the engine’s processing graph. See setManualRenderingInputPCMFormat(_:inputBlock:).

## See Also

### Constants

case error

A problem that occurs during rendering and results in no data returning.

case success

A status that indicates the successful return of the requested data.

case cannotDoInCurrentContext

An operation that the system can’t perform under the current conditions.

