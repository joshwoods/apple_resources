

- AVFAudio
- AVAudioSession
- AVAudioSession.PromptStyle
-  AVAudioSession.PromptStyle.short 

Case

# AVAudioSession.PromptStyle.short

Your app should issue short, nonverbal prompts.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
case short
```

## Discussion

The audio session’s prompt style is short when Siri is active but not recording, when a voicemail is playing back, or when a voice call is active.

## See Also

### Prompt Styles

case none

Your app shouldn’t issue prompts at this time.

case normal

Your app may use long, verbal prompts.

