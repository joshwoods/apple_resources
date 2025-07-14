

- AVFAudio
- AVMIDIPlayer
-  play(\_:) 

Instance Method

# play(\_:)

Plays the MIDI sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func play(_ completionHandler: AVMIDIPlayerCompletionHandler? = nil)
```

``` source
func play() async
```

## Parameters 

`completionHandler`  

A closure the system calls when playback completes.

## Topics

### Closures

typealias AVMIDIPlayerCompletionHandler

A callback the system invokes when MIDI playback completes.

## See Also

### Controlling playback

func prepareToPlay()

Prepares the player to play the sequence by prerolling all events.

func stop()

Stops playing the sequence.

var isPlaying: Bool

A Boolean value that indicates whether the sequence is playing.

