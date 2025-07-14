

- AVFAudio
- AVAudioPlayerNode
-  scheduleBuffer(\_:at:options:completionHandler:) 

Instance Method

# scheduleBuffer(\_:at:options:completionHandler:)

Schedules the playing samples from an audio buffer at the time and playback options you specify.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func scheduleBuffer(
    _ buffer: AVAudioPCMBuffer,
    at when: AVAudioTime?,
    options: AVAudioPlayerNodeBufferOptions = [],
    completionHandler: AVAudioNodeCompletionHandler? = nil
)
```

``` source
func scheduleBuffer(
    _ buffer: AVAudioPCMBuffer,
    at when: AVAudioTime?,
    options: AVAudioPlayerNodeBufferOptions = []
) async
```

## Parameters 

`buffer`  

The buffer to play.

`when`  

The time the buffer plays. For more information, see Scheduling Playback Time.

`options`  

The playback options that control buffer scheduling.

`completionHandler`  

The handler the system calls after the player schedules the buffer for playback on the render thread, or the player stops.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func scheduleBuffer(_ buffer: AVAudioPCMBuffer, at when: AVAudioTime?, options: AVAudioPlayerNodeBufferOptions = []) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Scheduling Playback

func scheduleFile(AVAudioFile, at: AVAudioTime?, completionHandler: AVAudioNodeCompletionHandler?)

Schedules the playing of an entire audio file.

func scheduleFile(AVAudioFile, at: AVAudioTime?, completionCallbackType: AVAudioPlayerNodeCompletionCallbackType, completionHandler: AVAudioPlayerNodeCompletionHandler?)

Schedules the playing of an entire audio file with a callback option you specify.

func scheduleSegment(AVAudioFile, startingFrame: AVAudioFramePosition, frameCount: AVAudioFrameCount, at: AVAudioTime?, completionHandler: AVAudioNodeCompletionHandler?)

Schedules the playing of an audio file segment.

func scheduleSegment(AVAudioFile, startingFrame: AVAudioFramePosition, frameCount: AVAudioFrameCount, at: AVAudioTime?, completionCallbackType: AVAudioPlayerNodeCompletionCallbackType, completionHandler: AVAudioPlayerNodeCompletionHandler?)

Schedules the playing of an audio file segment with a callback option you specify.

func scheduleBuffer(AVAudioPCMBuffer, completionHandler: AVAudioNodeCompletionHandler?)

Schedules the playing samples from an audio buffer.

func scheduleBuffer(AVAudioPCMBuffer, at: AVAudioTime?, options: AVAudioPlayerNodeBufferOptions, completionCallbackType: AVAudioPlayerNodeCompletionCallbackType, completionHandler: AVAudioPlayerNodeCompletionHandler?)

Schedules the playing samples from an audio buffer with the playback options you specify.

func scheduleBuffer(AVAudioPCMBuffer, completionCallbackType: AVAudioPlayerNodeCompletionCallbackType, completionHandler: AVAudioPlayerNodeCompletionHandler?)

Schedules the playing samples from an audio buffer with the callback option you specify.

struct AVAudioPlayerNodeBufferOptions

The buffer options that control the playback scheduling.

enum AVAudioPlayerNodeCompletionCallbackType

Constants that specify when the framework must invoke the completion handler.

typealias AVAudioPlayerNodeCompletionHandler

The callback handler for buffer or file completion.

