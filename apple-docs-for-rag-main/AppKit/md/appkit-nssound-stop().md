

- AppKit
- NSSound
-  stop() 

Instance Method

# stop()

Concludes audio playback.

macOS

``` source
func stop() -> Bool
```

## Return Value

true when playback is concluded successfully or if it’s paused, false otherwise.

## See Also

### Related Documentation

func sound(NSSound, didFinishPlaying: Bool)

This delegate method is called when an `NSSound` instance has completed playback of its sound data.

### Playing Sounds

static func beep()

Plays the system beep.

var isPlaying: Bool

A Boolean that indicates whether the sound is playing its audio data.

func pause() -> Bool

Pauses audio playback.

func play() -> Bool

Initiates audio playback.

func resume() -> Bool

Resumes audio playback.

