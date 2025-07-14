

- AVFAudio
- AVAudioPlayerNode
-  scheduleSegment(\_:startingFrame:frameCount:at:completionCallbackType:completionHandler:) 

Instance Method

# scheduleSegment(\_:startingFrame:frameCount:at:completionCallbackType:completionHandler:)

Schedules the playing of an audio file segment with a callback option you specify.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func scheduleSegment(
    _ file: AVAudioFile,
    startingFrame startFrame: AVAudioFramePosition,
    frameCount numberFrames: AVAudioFrameCount,
    at when: AVAudioTime?,
    completionCallbackType callbackType: AVAudioPlayerNodeCompletionCallbackType,
    completionHandler: AVAudioPlayerNodeCompletionHandler? = nil
)
```

``` source
func scheduleSegment(
    _ file: AVAudioFile,
    startingFrame startFrame: AVAudioFramePosition,
    frameCount numberFrames: AVAudioFrameCount,
    at when: AVAudioTime?,
    completionCallbackType callbackType: AVAudioPlayerNodeCompletionCallbackType
) async -> AVAudioPlayerNodeCompletionCallbackType
```

## Parameters 

`file`  

The file to play.

`startFrame`  

The starting frame position in the stream.

`numberFrames`  

The number of frames to play.

`when`  

The time the region plays.

`callbackType`  

The option to specify when the system must call the completion handler.

`completionHandler`  

The handler the system calls after the player schedules the segment for playback on the render thread, or the player stops.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func scheduleSegment(_ file: AVAudioFile, startingFrame startFrame: AVAudioFramePosition, frameCount numberFrames: AVAudioFrameCount, at when: AVAudioTime?, completionCallbackType callbackType: AVAudioPlayerNodeCompletionCallbackType) async -> AVAudioPlayerNodeCompletionCallbackType
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

func scheduleBuffer(AVAudioPCMBuffer, at: AVAudioTime?, options: AVAudioPlayerNodeBufferOptions, completionHandler: AVAudioNodeCompletionHandler?)

Schedules the playing samples from an audio buffer at the time and playback options you specify.

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

