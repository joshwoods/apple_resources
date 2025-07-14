

- PHASE
- PHASEPushStreamNode
-  scheduleBuffer(buffer:time:options:completionCallbackType:completionHandler:) 

Instance Method

# scheduleBuffer(buffer:time:options:completionCallbackType:completionHandler:)

Schedules audio data playback at a specific time with a completion handler.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func scheduleBuffer(
    buffer: AVAudioPCMBuffer,
    time when: AVAudioTime?,
    options: PHASEPushStreamBufferOptions = [],
    completionCallbackType: PHASEPushStreamCompletionCallbackCondition,
    completionHandler: @escaping (PHASEPushStreamCompletionCallbackCondition) -> Void
)
```

``` source
func scheduleBuffer(
    buffer: AVAudioPCMBuffer,
    time when: AVAudioTime?,
    options: PHASEPushStreamBufferOptions = [],
    completionCallbackType: PHASEPushStreamCompletionCallbackCondition
) async -> PHASEPushStreamCompletionCallbackCondition
```

## Parameters 

`buffer`  

Data that represents one portion of a contiguous audio stream.

`when`  

The time to play the buffer.

`options`  

The options for looping and buffer interruption.

`completionCallbackType`  

The specific event on which to handle completion.

`completionHandler`  

Code the framework runs on completion or when the player stops.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func scheduleBuffer(buffer: AVAudioPCMBuffer, time when: AVAudioTime?, options: PHASEPushStreamBufferOptions = [], completionCallbackType: PHASEPushStreamCompletionCallbackCondition) async -> PHASEPushStreamCompletionCallbackCondition
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Providing Audio Data

func scheduleBuffer(buffer: AVAudioPCMBuffer)

Schedules audio data for playback.

func scheduleBuffer(buffer: AVAudioPCMBuffer, time: AVAudioTime?, options: PHASEPushStreamBufferOptions)

Schedules audio data playback at a specific time.

func scheduleBuffer(buffer: AVAudioPCMBuffer, completionCallbackType: PHASEPushStreamCompletionCallbackCondition, completionHandler: (PHASEPushStreamCompletionCallbackCondition) -> Void)

Schedules audio data playback with a completion handler.

enum PHASEPushStreamCompletionCallbackCondition

A status that describes the results after the app schedules a push-stream buffer.

