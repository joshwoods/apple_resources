

- Application Services
- Speech Synthesis Manager
-  GetSpeechPitch(\_:\_:) Deprecated

Function

# GetSpeechPitch(\_:\_:)

Gets a speech channel’s current speech pitch.

macOS 10.0–13.0Deprecated

``` source
func GetSpeechPitch(
    _ chan: SpeechChannel,
    _ pitch: UnsafeMutablePointer
) -> OSErr
```

## Parameters 

`chan`  

The speech channel whose pitch you wish to determine.

`pitch`  

On return, a pointer to the current pitch of the voice in the speech channel, expressed as a fixed-point frequency value.

## Return Value

A resultcode. See Result Codes.

## Discussion

Typical voice frequencies range from around 90 hertz for alow-pitched male voice to perhaps 300 hertz for a high-pitched child’svoice. These frequencies correspond to approximate pitch valuesin the ranges of 30.000 to 40.000 and 55.000 to 65.000, respectively.

## See Also

### Obtaining Information About Speech and Speech Channels

func CopySpeechProperty(SpeechChannel, CFString, UnsafeMutablePointer&lt;CFTypeRef?>) -> OSErr

Gets the value associated with the specified property of a speech channel.

Deprecated

func GetSpeechRate(SpeechChannel, UnsafeMutablePointer&lt;Fixed>) -> OSErr

Gets a speech channel’s current speech rate.

Deprecated

func SpeechBusy() -> Int16

Determines whether any channels of speech are currentlysynthesizing speech.

Deprecated

func SpeechBusySystemWide() -> Int16

Determines if any speech is currently being synthesizedin your application or elsewhere on the computer.

Deprecated

func SpeechManagerVersion() -> NumVersion

Determines the current version of the Speech SynthesisManager installed in the system.

Deprecated

