

- Application Services
- Speech Synthesis Manager
-  ContinueSpeech(\_:) Deprecated

Function

# ContinueSpeech(\_:)

Resumes speech paused by the `PauseSpeechAt` function.

macOS 10.0–13.0Deprecated

``` source
func ContinueSpeech(_ chan: SpeechChannel) -> OSErr
```

## Parameters 

`chan`  

The paused speech channel on which speech is to be resumed.

## Return Value

A resultcode. See Result Codes.

## Discussion

At any time after the `PauseSpeechAt` functionis called, the `ContinueSpeech` functioncan be called to continue speaking from the beginning of the wordin which speech paused. Calling `ContinueSpeech` ona channel that is not currently in a paused state has no effecton the speech channel or on future calls to the `PauseSpeechAt` function.If you call `ContinueSpeech` ona channel before a pause is effective, `ContinueSpeech` cancelsthe pause.

If the `PauseSpeechAt` functionstopped speech in the middle of a word, the Speech Synthesis Managerwill start speaking that word from the beginning when you call `ContinueSpeech`.

## See Also

### Starting, Stopping, and Pausing Speech

func PauseSpeechAt(SpeechChannel, Int32) -> OSErr

Pauses speech on a speech channel.

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

