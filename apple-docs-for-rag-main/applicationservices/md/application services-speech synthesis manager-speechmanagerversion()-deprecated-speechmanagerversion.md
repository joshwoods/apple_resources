

- Application Services
- Speech Synthesis Manager
-  SpeechManagerVersion() Deprecated

Function

# SpeechManagerVersion()

Determines the current version of the Speech SynthesisManager installed in the system.

macOS 10.0–13.0Deprecated

``` source
func SpeechManagerVersion() -> NumVersion
```

## Return Value

The version of theSpeech Synthesis Manager installed in the system, in the formatof the first 4 bytes of a `'vers'` resource.

## Discussion

Use this call to determine whether your program can accessfeatures of the Speech Synthesis Manager that are included in someSpeech Synthesis Manager releases but not in earlier ones.

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

func SpeechBusySystemWide() -> Int16

Determines if any speech is currently being synthesizedin your application or elsewhere on the computer.

Deprecated

