

- Application Services
- Speech Synthesis Manager
-  NewSpeechChannel(\_:\_:) Deprecated

Function

# NewSpeechChannel(\_:\_:)

Creates a new speech channel.

macOS 10.0–13.0Deprecated

``` source
func NewSpeechChannel(
    _ voice: UnsafeMutablePointer?,
    _ chan: UnsafeMutablePointer
) -> OSErr
```

## Parameters 

`voice`  

A pointer to the voice specification structure corresponding to the voice to be used for the new speech channel. Pass `NULL` to create a speech channel using the system default voice.

Specifying a voice means the initial speaking rate is determined by the synthesizer’s default speaking rate; passing `NULL` means the speaking rate is automatically set to the rate the user specifies in Speech preferences.

`chan`  

On return, a pointer to a valid speech channel.

## Return Value

A result code. See Result Codes.

## Discussion

The `NewSpeechChannel` functionallocates memory for a speech channel structure and sets the speechchannel variable pointed to by the `chan` parameterto point to this speech channel structure. The Speech SynthesisManager automatically locates and opens a connection to the propersynthesizer for the voice specified by the `voice` parameter.

There is no predefined limit to the number of speech channelsan application can create. However, system constraints on availableRAM, processor loading, and number of available sound channels limitthe number of speech channels actually possible.

Your application should not attempt to manipulate the datapointed to by a variable of type `SpeechChannel`.The internal format that the Speech Synthesis Manager uses for speech channeldata is not documented and may change in future versions of systemsoftware.

## See Also

### Managing Speech Channels

func DisposeSpeechChannel(SpeechChannel) -> OSErr

Disposes of an existing speech channel.

Deprecated

