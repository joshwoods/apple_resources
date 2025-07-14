

- AppKit
- NSSound
-  play() 

Instance Method

# play()

Initiates audio playback.

macOS

``` source
func play() -> Bool
```

## Return Value

true when playback is initiated, false when playback is already in progress or when an error occurred.

## Discussion

This method initiates playback asynchronously and returns control to your application. Therefore, your application can continue doing work while the audio is playing.

## See Also

### Playing Sounds

static func beep()

Plays the system beep.

var isPlaying: Bool

A Boolean that indicates whether the sound is playing its audio data.

func pause() -> Bool

Pauses audio playback.

func resume() -> Bool

Resumes audio playback.

func stop() -> Bool

Concludes audio playback.

