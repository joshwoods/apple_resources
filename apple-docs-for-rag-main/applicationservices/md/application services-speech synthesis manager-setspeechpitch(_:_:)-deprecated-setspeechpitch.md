

- Application Services
- Speech Synthesis Manager
-  SetSpeechPitch(\_:\_:) Deprecated

Function

# SetSpeechPitch(\_:\_:)

Sets the speech pitch on a designated speech channel.

macOS 10.0–13.0Deprecated

``` source
func SetSpeechPitch(
    _ chan: SpeechChannel,
    _ pitch: Fixed
) -> OSErr
```

## Parameters 

`chan`  

The speech channel whose pitch you wish to set.

`pitch`  

The new pitch for the speech channel, expressed as a fixed-point frequency value.

## Return Value

A resultcode. See Result Codes.

## Discussion

The `SetSpeechPitch` functionchanges the current speech pitch on the speech channel specifiedby the `chan` parameterto the pitch specified by the `pitch` parameter.Typical voice frequencies range from around 90 hertz for a low-pitchedmale voice to perhaps 300 hertz for a high-pitched child’s voice.These frequencies correspond to approximate pitch values in theranges of 30.000 to 40.000 and 55.000 to 65.000, respectively. Althoughfixed-point values allow you to specify a wide range of pitches,not all synthesizers will support the full range of pitches. Ifyour application specifies a pitch that a synthesizer cannot handle, itmay adjust the pitch to fit within an acceptable range.

## See Also

### Changing Speech Attributes

func SetSpeechProperty(SpeechChannel, CFString, CFTypeRef?) -> OSErr

Sets the value of the specified speech-channel property.

Deprecated

func SetSpeechRate(SpeechChannel, Fixed) -> OSErr

Sets the speech rate of a designated speech channel.

Deprecated

