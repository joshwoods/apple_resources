

- Application Services
- Speech Synthesis Manager
-  SpeakCFString(\_:\_:\_:) Deprecated

Function

# SpeakCFString(\_:\_:\_:)

Begins speaking a string represented as a `CFString` object.

macOS 10.5–13.0Deprecated

``` source
func SpeakCFString(
    _ chan: SpeechChannel,
    _ aString: CFString,
    _ options: CFDictionary?
) -> OSErr
```

## Parameters 

`chan`  

The speech channel through which speech is to be spoken.

`aString`  

The string to be spoken, represented as a `CFString` object.

`options`  

An optional dictionary of key-value pairs used to customize speech behavior. See Synthesizer Option Keys for the available keys.

## Return Value

A result code. See Result Codes.

## Discussion

The `SpeakCFString` function is the Core Foundation-based equivalent of the SpeakBuffer function.

The `SpeakCFString` function converts the text string specified in `aString` into speech, using the voice and control settings in effect for the speech channel specified in `chan`. (Before you use `SpeakCFString`, therefore, be sure you’ve created a speech channel with the NewSpeechChannel(_:_:) function.) The `SpeakCFString` function generates speech asynchronously, which means that control is returned to your application before speech has finished, perhaps even before the speech is first audible.

If `SpeakCFString` is called while the speech channel is currently speaking the contents of another text string, the speech stops immediately and the new text string is spoken as soon as possible.

## See Also

### Starting, Stopping, and Pausing Speech

func ContinueSpeech(SpeechChannel) -> OSErr

Resumes speech paused by the `PauseSpeechAt` function.

Deprecated

func PauseSpeechAt(SpeechChannel, Int32) -> OSErr

Pauses speech on a speech channel.

Deprecated

func StopSpeech(SpeechChannel) -> OSErr

Terminates speech immediately on the specified channel.

Deprecated

func StopSpeechAt(SpeechChannel, Int32) -> OSErr

Terminates speech delivery on a specified channel eitherimmediately or at the end of the current word or sentence.

Deprecated

