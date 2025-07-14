

- Application Services
- Speech Synthesis Manager
-  CopySpeechProperty(\_:\_:\_:) Deprecated

Function

# CopySpeechProperty(\_:\_:\_:)

Gets the value associated with the specified property of a speech channel.

macOS 10.5–13.0Deprecated

``` source
func CopySpeechProperty(
    _ chan: SpeechChannel,
    _ property: CFString,
    _ object: UnsafeMutablePointer
) -> OSErr
```

## Parameters 

`chan`  

The speech channel with which the specified property is associated.

`property`  

A speech-channel property about which information is being requested. See Speech-Channel Properties for information on the properties you can specify.

`object`  

On return, a pointer to a Core Foundation object that holds the value of the specified property. The type of the object depends on the specific property passed in. For some properties, the value of `object` can be `NULL`. When the returned object is a `CFDictionary` object, you can use `CFDictionary` functions, such as CFDictionaryGetValue(_:_:), to retrieve the values associated with the keys that are associated with the specified property.

## Return Value

A result code. See Result Codes.

## Discussion

The `CopySpeechProperty` function is the Core Foundation-based equivalent of the GetSpeechInfo function.

## See Also

### Obtaining Information About Speech and Speech Channels

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

func SpeechManagerVersion() -> NumVersion

Determines the current version of the Speech SynthesisManager installed in the system.

Deprecated

