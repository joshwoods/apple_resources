

- Application Services
- Speech Synthesis Manager
-  SpeechBusy() Deprecated

Function

# SpeechBusy()

Determines whether any channels of speech are currentlysynthesizing speech.

macOS 10.0–13.0Deprecated

``` source
func SpeechBusy() -> Int16
```

## Return Value

The number of speechchannels that are currently synthesizing speech in the application.This is useful when you want to ensure that an earlier speech requesthas been completed before having the system speak again. Pausedspeech channels are counted among those that are synthesizing speech.

The speech channel that the Speech Synthesis Manager allocatesinternally in response to calls to the `SpeakString` functionis counted in the number returned by `SpeechBusy`. Thus,if you use just `SpeakString` toinitiate speech, `SpeechBusy` alwaysreturns `1` as long as speech is being produced. When `SpeechBusy` returns`0`, all speech has finished.

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

func SpeechBusySystemWide() -> Int16

Determines if any speech is currently being synthesizedin your application or elsewhere on the computer.

Deprecated

func SpeechManagerVersion() -> NumVersion

Determines the current version of the Speech SynthesisManager installed in the system.

Deprecated

