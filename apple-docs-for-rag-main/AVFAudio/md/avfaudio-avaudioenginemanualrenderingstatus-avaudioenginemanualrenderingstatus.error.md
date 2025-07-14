

- AVFAudio
- AVAudioEngineManualRenderingStatus
-  AVAudioEngineManualRenderingStatus.error 

Case

# AVAudioEngineManualRenderingStatus.error

A problem that occurs during rendering and results in no data returning.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
case error
```

## See Also

### Constants

case success

A status that indicates the successful return of the requested data.

case insufficientDataFromInputNode

A condition that occurs when the input node doesn’t return enough input data to satisfy the render request at the time of the request.

case cannotDoInCurrentContext

An operation that the system can’t perform under the current conditions.

