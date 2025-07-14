

- AVFAudio
- AVAudioPlayerNode
-  isPlaying 

Instance Property

# isPlaying

A Boolean value that indicates whether the player is playing.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isPlaying: Bool { get }
```

## See Also

### Controlling Playback

func prepare(withFrameCount: AVAudioFrameCount)

Prepares the file regions or buffers you schedule for playback.

func play()

Starts or resumes playback immediately.

func play(at: AVAudioTime?)

Starts or resumes playback at a time you specify.

func pause()

Pauses the node’s playback.

func stop()

Clears all of the node’s events you schedule and stops playback.

