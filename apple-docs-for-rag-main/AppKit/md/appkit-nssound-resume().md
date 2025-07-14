

- AppKit
- NSSound
-  resume() 

Instance Method

# resume()

Resumes audio playback.

macOS

``` source
func resume() -> Bool
```

## Return Value

true when playback is resumed, false when playback is in progress or when an error occurred.

## Discussion

Assumes the receiver has been previously paused by sending it NSSound.

## See Also

### Playing Sounds

static func beep()

Plays the system beep.

var isPlaying: Bool

A Boolean that indicates whether the sound is playing its audio data.

func pause() -> Bool

Pauses audio playback.

func play() -> Bool

Initiates audio playback.

func stop() -> Bool

Concludes audio playback.

