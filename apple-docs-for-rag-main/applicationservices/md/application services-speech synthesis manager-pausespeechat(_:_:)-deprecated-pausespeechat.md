

- Application Services
- Speech Synthesis Manager
-  PauseSpeechAt(\_:\_:) Deprecated

Function

# PauseSpeechAt(\_:\_:)

Pauses speech on a speech channel.

macOS 10.0–13.0Deprecated

``` source
func PauseSpeechAt(
    _ chan: SpeechChannel,
    _ whereToPause: Int32
) -> OSErr
```

## Parameters 

`chan`  

The speech channel on which speech is to be paused.

`whereToPause`  

A constant indicating when speech processing should be paused. Pass the constant `kImmediate` to pause immediately, even in the middle of a word. Pass `kEndOfWord` or `kEndOfSentence` to pause speech at the end of the current word or sentence, respectively.

## Return Value

A resultcode. See Result Codes.

## Discussion

The `PauseSpeechAt` functionmakes speech production pause at a specified point in the text. `PauseSpeechAt` returnsimmediately, although speech output will continue until the specifiedpoint.

You can determine whether your application has paused speechoutput on a speech channel by obtaining a speech status informationstructure through the `GetSpeechInfo` function.While a speech channel is paused, the speech status informationstructure indicates that `outputBusy` and `outputPaused` areboth `TRUE`.

If the end of the input text buffer is reached before thespecified pause point, speech output pauses at the end of the buffer.

The `PauseSpeechAt` functiondiffers from the `StopSpeech` and `StopSpeechAt` functionsin that a subsequent call to `ContinueSpeech`,described next, causes the contents of the current text buffer tocontinue being spoken.

If you plan to continue speech synthesis from a paused speechchannel, the text buffer being processed must remain available atall times and must not move while the channel is in a paused state.

## See Also

### Starting, Stopping, and Pausing Speech

func ContinueSpeech(SpeechChannel) -> OSErr

Resumes speech paused by the `PauseSpeechAt` function.

Deprecated

func SpeakCFString(SpeechChannel, CFString, CFDictionary?) -> OSErr

Begins speaking a string represented as a `CFString` object.

Deprecated

func StopSpeech(SpeechChannel) -> OSErr

Terminates speech immediately on the specified channel.

Deprecated

func StopSpeechAt(SpeechChannel, Int32) -> OSErr

Terminates speech delivery on a specified channel eitherimmediately or at the end of the current word or sentence.

Deprecated

