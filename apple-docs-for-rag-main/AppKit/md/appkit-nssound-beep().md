

- AppKit
- NSSound
-  beep() 

Type Method

# beep()

Plays the system beep.

macOS 10.9+Swift 4.0+

``` source
static func beep()
```

## Discussion

Users can select a sound to be played as the system beep in the Sound pane of System Preferences.

## See Also

### Playing Sounds

var isPlaying: Bool

A Boolean that indicates whether the sound is playing its audio data.

func pause() -> Bool

Pauses audio playback.

func play() -> Bool

Initiates audio playback.

func resume() -> Bool

Resumes audio playback.

func stop() -> Bool

Concludes audio playback.

