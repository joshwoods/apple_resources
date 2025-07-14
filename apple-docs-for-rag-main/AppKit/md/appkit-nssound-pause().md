

- AppKit
- NSSound
-  pause() 

Instance Method

# pause()

Pauses audio playback.

macOS

``` source
func pause() -> Bool
```

## Return Value

true when playback is paused successfully, false when playback is already paused or when an error occurred.

## See Also

### Playing Sounds

static func beep()

Plays the system beep.

var isPlaying: Bool

A Boolean that indicates whether the sound is playing its audio data.

func play() -> Bool

Initiates audio playback.

func resume() -> Bool

Resumes audio playback.

func stop() -> Bool

Concludes audio playback.

