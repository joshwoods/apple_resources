

- Application Services
- Speech Synthesis Manager
-  SetSpeechRate(\_:\_:) Deprecated

Function

# SetSpeechRate(\_:\_:)

Sets the speech rate of a designated speech channel.

macOS 10.0–13.0Deprecated

``` source
func SetSpeechRate(
    _ chan: SpeechChannel,
    _ rate: Fixed
) -> OSErr
```

## Parameters 

`chan`  

The speech channel whose rate you wish to set.

`rate`  

The new speech rate in words per minute, expressed as an integer value.

## Return Value

A resultcode. See Result Codes.

## Discussion

The `SetSpeechRate` functionadjusts the speech rate on the speech channel specified by the `chan` parameterto the rate specified by the `rate` parameter.As a general rule, speaking rates range from around 150 words perminute to around 220 words per minute. It is important to keep inmind, however, that users will differ greatly in their ability to understandsynthesized speech at a particular rate based upon their level ofexperience listening to the voice and their ability to anticipatethe types of utterances they will encounter.

Note: the new speech rate should be expressed as an integer (nota fixed point decimal number as the data type implies).

## See Also

### Changing Speech Attributes

func SetSpeechProperty(SpeechChannel, CFString, CFTypeRef?) -> OSErr

Sets the value of the specified speech-channel property.

Deprecated

func SetSpeechPitch(SpeechChannel, Fixed) -> OSErr

Sets the speech pitch on a designated speech channel.

Deprecated

