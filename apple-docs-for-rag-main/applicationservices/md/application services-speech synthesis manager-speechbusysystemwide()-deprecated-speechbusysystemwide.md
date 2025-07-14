

- Application Services
- Speech Synthesis Manager
-  SpeechBusySystemWide() Deprecated

Function

# SpeechBusySystemWide()

Determines if any speech is currently being synthesizedin your application or elsewhere on the computer.

macOS 10.0–13.0Deprecated

``` source
func SpeechBusySystemWide() -> Int16
```

## Return Value

The total number ofspeech channels currently synthesizing speech on the computer, whetherthey were initiated by your application or process’s code or bysome other process executing concurrently. Paused speech channelsare counted among those channels that are synthesizing speech.

## Discussion

This function is useful when you want to ensure that no speechis currently being produced anywhere on the Macintosh computer beforeinitiating speech. Although the Speech Synthesis Manager allowsdifferent applications to produce speech simultaneously, this canbe confusing to the user. As a result, it is often a good idea foryour application to check that no other process is producing speechbefore producing speech itself. If the difference between the valuesreturned by `SpeechBusySystemWide` andthe `SpeechBusy` functionis `0`, no other process is producing speech.

## See Also

### Obtaining Information About Speech and Speech Channels

func CopySpeechProperty(SpeechChannel, CFString, UnsafeMutablePointer&lt;CFTypeRef?>) -> OSErr

Gets the value associated with the specified property of a speech channel.

Deprecated

func GetSpeechPitch(SpeechChannel, UnsafeMutablePointer&lt;Fixed>) -> OSErr

Gets a speech channel’s current speech pitch.

Deprecated

func GetSpeechRate(SpeechChannel, UnsafeMutablePointer&lt;Fixed>) -> OSErr

Gets a speech channel’s current speech rate.

Deprecated

func SpeechBusy() -> Int16

Determines whether any channels of speech are currentlysynthesizing speech.

Deprecated

func SpeechManagerVersion() -> NumVersion

Determines the current version of the Speech SynthesisManager installed in the system.

Deprecated

