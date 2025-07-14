

- Audio Toolbox
-  AudioServicesPlaySystemSoundWithCompletion(\_:\_:) 

Function

# AudioServicesPlaySystemSoundWithCompletion(\_:\_:)

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func AudioServicesPlaySystemSoundWithCompletion(
    _ inSystemSoundID: SystemSoundID,
    _ inCompletionBlock: (() -> Void)?
)
```

## See Also

### Playing Sounds

func AudioServicesPlayAlertSoundWithCompletion(SystemSoundID, (() -> Void)?)

func AudioServicesPlayAlertSound(SystemSoundID)

Plays a system sound as an alert.

func AudioServicesPlaySystemSound(SystemSoundID)

Plays a system sound object.

