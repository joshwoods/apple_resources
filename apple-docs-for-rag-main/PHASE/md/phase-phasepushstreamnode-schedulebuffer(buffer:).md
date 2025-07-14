

- PHASE
- PHASEPushStreamNode
-  scheduleBuffer(buffer:) 

Instance Method

# scheduleBuffer(buffer:)

Schedules audio data for playback.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func scheduleBuffer(buffer: AVAudioPCMBuffer)
```

## Parameters 

`buffer`  

Data that represents one portion of a contiguous audio stream.

## Discussion

The framework processes this buffer after completing previously scheduled buffers. The buffer’s data format needs to match format.

## See Also

### Providing Audio Data

func scheduleBuffer(buffer: AVAudioPCMBuffer, time: AVAudioTime?, options: PHASEPushStreamBufferOptions)

Schedules audio data playback at a specific time.

func scheduleBuffer(buffer: AVAudioPCMBuffer, time: AVAudioTime?, options: PHASEPushStreamBufferOptions, completionCallbackType: PHASEPushStreamCompletionCallbackCondition, completionHandler: (PHASEPushStreamCompletionCallbackCondition) -> Void)

Schedules audio data playback at a specific time with a completion handler.

func scheduleBuffer(buffer: AVAudioPCMBuffer, completionCallbackType: PHASEPushStreamCompletionCallbackCondition, completionHandler: (PHASEPushStreamCompletionCallbackCondition) -> Void)

Schedules audio data playback with a completion handler.

enum PHASEPushStreamCompletionCallbackCondition

A status that describes the results after the app schedules a push-stream buffer.

