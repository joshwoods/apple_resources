

- Application Services
- Speech Synthesis Manager
-  GetSpeechRate(\_:\_:) Deprecated

Function

# GetSpeechRate(\_:\_:)

Gets a speech channel’s current speech rate.

macOS 10.0–13.0Deprecated

``` source
func GetSpeechRate(
    _ chan: SpeechChannel,
    _ rate: UnsafeMutablePointer
) -> OSErr
```

## Parameters 

`chan`  

The speech channel whose rate you wish to determine.

`rate`  

On return, a pointer to the speech channel’s speech rate in words per minute, expressed as an integer value.

## Return Value

A resultcode. See Result Codes.

## See Also

### Obtaining Information About Speech and Speech Channels

func CopySpeechProperty(SpeechChannel, CFString, UnsafeMutablePointer&lt;CFTypeRef?>) -> OSErr

Gets the value associated with the specified property of a speech channel.

Deprecated

func GetSpeechPitch(SpeechChannel, UnsafeMutablePointer&lt;Fixed>) -> OSErr

Gets a speech channel’s current speech pitch.

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

