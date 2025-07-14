

- AVFAudio
- AVAudioSession
-  AVAudioSession.PromptStyle 

Enumeration

# AVAudioSession.PromptStyle

Constants that indicate the prompt style to use.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
enum PromptStyle
```

## Topics

### Prompt Styles

case none

Your app shouldn’t issue prompts at this time.

case short

Your app should issue short, nonverbal prompts.

case normal

Your app may use long, verbal prompts.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting the audio prompt style

var promptStyle: AVAudioSession.PromptStyle

A hint to audio sessions that use voice prompt mode to alter the type of prompts they issue in response to other system audio, such as Siri and phone calls.

