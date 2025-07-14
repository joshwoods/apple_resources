

- AVFAudio
- AVAudioPlayerNode
-  play(at:) 

Instance Method

# play(at:)

Starts or resumes playback at a time you specify.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func play(at when: AVAudioTime?)
```

## Parameters 

`when`  

The node time to start or resume playback. Passing `nil` starts playback immediately.

## Discussion

This node is initially in a paused state. The framework enqueues your requests to play buffers or file segments, and any necessary decoding begins immediately. Playback doesn’t begin until the player starts playing through this method.

The following example code shows how to start a player `0.5` seconds in the future:

```
// Start the engine and player.
NSError *nsErr = nil;
[_engine startAndReturnError:&nsErr];
if (!nsErr) {
    const float kStartDelayTime = 0.5; // sec
    AVAudioFormat *outputFormat = [_player outputFormatForBus:0];
    AVAudioFramePosition startSampleTime = _player.lastRenderTime.sampleTime + kStartDelayTime * outputFormat.sampleRate;
    AVAudioTime *startTime = [AVAudioTime timeWithSampleTime:startSampleTime atRate:outputFormat.sampleRate];
    [_player playAtTime:startTime];
}
```

## See Also

### Controlling Playback

func prepare(withFrameCount: AVAudioFrameCount)

Prepares the file regions or buffers you schedule for playback.

func play()

Starts or resumes playback immediately.

var isPlaying: Bool

A Boolean value that indicates whether the player is playing.

func pause()

Pauses the node’s playback.

func stop()

Clears all of the node’s events you schedule and stops playback.

