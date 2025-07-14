

- Audio Toolbox
-  AudioComponentValidate(\_:\_:\_:) 

Function

# AudioComponentValidate(\_:\_:\_:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.7+visionOS 1.0+

``` source
func AudioComponentValidate(
    _ inComponent: AudioComponent,
    _ inValidationParameters: CFDictionary?,
    _ outValidationResult: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Validating an Audio Component

var kAudioComponentValidationParameter_LoadOutOfProcess: String

enum AudioComponentValidationResult

