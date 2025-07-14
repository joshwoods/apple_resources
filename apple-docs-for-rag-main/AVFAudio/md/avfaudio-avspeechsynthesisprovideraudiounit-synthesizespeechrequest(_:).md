

- AVFAudio
- AVSpeechSynthesisProviderAudioUnit
-  synthesizeSpeechRequest(\_:) 

Instance Method

# synthesizeSpeechRequest(\_:)

Sets the text to synthesize and the voice to use.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func synthesizeSpeechRequest(_ speechRequest: AVSpeechSynthesisProviderRequest)
```

## Parameters 

`speechRequest`  

A speech request to synthesize.

## Discussion

When the synthesizer finishes generating audio buffers for the speech request, use AUInternalRenderBlock to report offlineUnitRenderAction_Complete.

## See Also

### Rendering speech

class AVSpeechSynthesisProviderRequest

An object that represents the text to synthesize and the voice to use.

