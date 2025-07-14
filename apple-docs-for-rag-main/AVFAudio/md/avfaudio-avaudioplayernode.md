

- AVFAudio
-  AVAudioPlayerNode 

Class

# AVAudioPlayerNode

An object for scheduling the playback of buffers or segments of audio files.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioPlayerNode
```

## Overview

This audio node supports scheduling the playback of AVAudioPCMBuffer instances, or segments of audio files that you open through AVAudioFile. You can schedule buffers and segments to play at specific points in time or to play immediately following preceding segments.

Generally, you want to configure the node’s output format with the same number of channels as in the files and buffers. Otherwise, the node drops or adds channels as necessary. It’s usually preferable to use an AVAudioMixerNode for this configuration.

Similarly, when playing file segments, the node makes sample rate conversions, if necessary. It’s preferable to configure the node’s output sample rate to match that of the files, and to use a mixer to perform the rate conversion.

When playing buffers, there’s an implicit assumption that the buffers are at the same sample rate as the node’s output format.

The stop() method unschedules all previously scheduled buffers and file segments, and returns the player timeline to sample time `0`.

Note

The `AVAudioPlayerNode` class isn’t key-value observing compliant, and may indicate that Combine publishers are available. Don’t use them for monitoring changes.

### Player Timeline

The usual AVAudioNode sample times, which lastRenderTime observes, have an arbitrary zero point. The `AVAudioPlayerNode` class superimposes a second player timeline on top of this to reflect when the player starts and intervals when it pauses. The methods nodeTime(forPlayerTime:) and playerTime(forNodeTime:) convert between the two.

### Scheduling Playback Time

The scheduleBuffer(_:at:options:completionHandler:), scheduleFile(_:at:completionHandler:), and scheduleSegment(_:startingFrame:frameCount:at:completionHandler:) methods take an AVAudioTime `when` parameter, and you interpret it as follows:

- If the `when` parameter is `nil`:

- If there are previous commands, the new one plays immediately following the last one.

- Otherwise, if the node is in a playing state, the event plays in the very near future.

- Otherwise, the command plays at sample time `0`.

- If the `when` parameter is a sample time, the parameter interprets it as such.

- If the `when` parameter is a host time, the system ignores it unless the sample time is invalid when the engine is rendering to an audio device.

The scheduling methods fail if:

- A buffer’s channel count doesn’t match that of the node’s output format.

- The system can’t access a file.

- An AVAudioTime doesn’t specify a valid sample time or a host time.

- A segment’s start frame or frame count is a negative value.

### Handling Buffer or File Completion

The buffer of file completion handlers are a means to schedule more data if available on the player node. For more information on the different completion callback types, see AVAudioPlayerNodeCompletionCallbackType.

Important

Don’t stop a player within a completion handler callback because it can deadlock while trying to unschedule already scheduled buffers.

### Rendering Offline

When you use a player node with the engine operating in manual rendering mode, you use the buffer or file completion handlers — lastRenderTime, latency, and outputPresentationLatency — to track how much data the player rendered and how much remains to render.

## Topics

### Creating a Player Node

init()

Creates an initialized audio player node.

### Scheduling Playback

func scheduleFile(AVAudioFile, at: AVAudioTime?, completionHandler: AVAudioNodeCompletionHandler?)

Schedules the playing of an entire audio file.

func scheduleFile(AVAudioFile, at: AVAudioTime?, completionCallbackType: AVAudioPlayerNodeCompletionCallbackType, completionHandler: AVAudioPlayerNodeCompletionHandler?)

Schedules the playing of an entire audio file with a callback option you specify.

func scheduleSegment(AVAudioFile, startingFrame: AVAudioFramePosition, frameCount: AVAudioFrameCount, at: AVAudioTime?, completionHandler: AVAudioNodeCompletionHandler?)

Schedules the playing of an audio file segment.

func scheduleSegment(AVAudioFile, startingFrame: AVAudioFramePosition, frameCount: AVAudioFrameCount, at: AVAudioTime?, completionCallbackType: AVAudioPlayerNodeCompletionCallbackType, completionHandler: AVAudioPlayerNodeCompletionHandler?)

Schedules the playing of an audio file segment with a callback option you specify.

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

### Converting Node and Player Times

func nodeTime(forPlayerTime: AVAudioTime) -> AVAudioTime?

Converts from player time to node time.

func playerTime(forNodeTime: AVAudioTime) -> AVAudioTime?

Converts from node time to player time.

### Controlling Playback

func prepare(withFrameCount: AVAudioFrameCount)

Prepares the file regions or buffers you schedule for playback.

func play()

Starts or resumes playback immediately.

func play(at: AVAudioTime?)

Starts or resumes playback at a time you specify.

var isPlaying: Bool

A Boolean value that indicates whether the player is playing.

func pause()

Pauses the node’s playback.

func stop()

Clears all of the node’s events you schedule and stops playback.

## Relationships

### Inherits From

- AVAudioNode

### Conforms To

- AVAudio3DMixing
- AVAudioMixing
- AVAudioStereoMixing
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Playback

Playing custom audio with your own player

Construct an audio player to play your custom audio data, and optionally take advantage of the advanced features of AirPlay 2.

Using voice processing

Add voice-processing capabilities to your app by using audio engine.

