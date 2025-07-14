

- AVFAudio
- AVAudioPlayerNode
-  prepare(withFrameCount:) 

Instance Method

# prepare(withFrameCount:)

Prepares the file regions or buffers you schedule for playback.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func prepare(withFrameCount frameCount: AVAudioFrameCount)
```

## Parameters 

`frameCount`  

The number of sample frames of data to prepare.

## See Also

### Controlling Playback

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

