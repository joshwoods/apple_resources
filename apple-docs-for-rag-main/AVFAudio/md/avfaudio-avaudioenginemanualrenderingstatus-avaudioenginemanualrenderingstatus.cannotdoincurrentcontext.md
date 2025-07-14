

- AVFAudio
- AVAudioEngineManualRenderingStatus
-  AVAudioEngineManualRenderingStatus.cannotDoInCurrentContext 

Case

# AVAudioEngineManualRenderingStatus.cannotDoInCurrentContext

An operation that the system can’t perform under the current conditions.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
case cannotDoInCurrentContext
```

## Discussion

This status guards a real-time render operation when a reconfiguration of the engine’s internal state is in progress. The client can try again later.

## See Also

### Constants

case error

A problem that occurs during rendering and results in no data returning.

case success

A status that indicates the successful return of the requested data.

case insufficientDataFromInputNode

A condition that occurs when the input node doesn’t return enough input data to satisfy the render request at the time of the request.

