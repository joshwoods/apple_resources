

- AVFAudio
- AVAudioSession
- AVAudioSession.PromptStyle
-  AVAudioSession.PromptStyle.none 

Case

# AVAudioSession.PromptStyle.none

Your app shouldn’t issue prompts at this time.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
case none
```

## Discussion

This style indicates that another audio session is currently using microphone input, and your app shouldn’t issue prompts at this time.

For example, if Siri is recognizing speech, playing navigation or exercise prompts could interfere with Siri’s ability to accurately recognize the user’s speech. Your app should refrain from playing any prompts while the prompt style equals this value.

## See Also

### Prompt Styles

case short

Your app should issue short, nonverbal prompts.

case normal

Your app may use long, verbal prompts.

