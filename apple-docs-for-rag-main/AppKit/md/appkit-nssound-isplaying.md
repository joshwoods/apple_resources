

- AppKit
- NSSound
-  isPlaying 

Instance Property

# isPlaying

A Boolean that indicates whether the sound is playing its audio data.

macOS

``` source
var isPlaying: Bool { get }
```

## Discussion

The value of this property is true when the receiver is playing its audio data.

## See Also

### Playing Sounds

static func beep()

Plays the system beep.

func pause() -> Bool

Pauses audio playback.

func play() -> Bool

Initiates audio playback.

func resume() -> Bool

Resumes audio playback.

func stop() -> Bool

Concludes audio playback.

