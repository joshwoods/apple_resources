

- Application Services
- Speech Synthesis Manager
-  SpeechSynthesisUnregisterModuleURL(\_:) Deprecated

Function

# SpeechSynthesisUnregisterModuleURL(\_:)

Unregisters a registered speech synthesizer or voice.

macOS 10.6–13.0Deprecated

``` source
func SpeechSynthesisUnregisterModuleURL(_ url: CFURL) -> OSErr
```

## Parameters 

`url`  

The file URL of the synthesizer plug-in or voice to unregister.

## Return Value

A resultcode. See Result Codes.

## Discussion

The `SpeechSynthesisUnregisterModuleURL` function unregisters the speech synthesizer or voice specified by `url`. When a synthesizer is unregistered, all voices that require that synthesizer are automatically unregistered.

Note that if a speech channel is currently using a synthesizer or voice that becomes unregistered, the speech channel is considered inactive and will return an error when the application tries to access it.

An application that called SpeechSynthesisRegisterModuleURL(_:) to register a synthesizer or voice should do the following if the volume containing the synthesizer or voice is about to be unmounted:

- Call DisposeSpeechChannel(_:) to dispose of each speech channel that uses the synthesizer or voice

- Call `SpeechSynthesisUnregisterModuleURL` to unregister the synthesizer or voice

If you call `SpeechSynthesisUnregisterModuleURL` to unregister a synthesizer or voice and you receive either the noSynthFound or voiceNotFound result codes, it means that the synthesizer or voice is not currently registered.

## See Also

### Registering and Unregistering Synthesizers and Voices

func SpeechSynthesisRegisterModuleURL(CFURL) -> OSErr

Registers and makes available a speech synthesizer or voice.

Deprecated

