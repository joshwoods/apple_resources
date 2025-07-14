

- Application Services
- Speech Synthesis Manager
-  StopSpeechAt(\_:\_:) Deprecated

Function

# StopSpeechAt(\_:\_:)

Terminates speech delivery on a specified channel eitherimmediately or at the end of the current word or sentence.

macOS 10.0–13.0Deprecated

``` source
func StopSpeechAt(
    _ chan: SpeechChannel,
    _ whereToStop: Int32
) -> OSErr
```

## Parameters 

`chan`  

The speech channel on which speech is to be stopped.

`whereToStop`  

A constant indicating when speech processing should stop. Pass the constant `kImmediate` to stop immediately, even in the middle of a word. Pass `kEndOfWord` or `kEndOfSentence` to stop speech at the end of the current word or sentence, respectively.

## Return Value

A resultcode. See Result Codes.

## Discussion

The `StopSpeechAt` functionhalts the production of speech on the channel specified by `chan` ata specified point in the text. This function returns immediately,although speech output continues until the specified point has beenreached.

If you call the `StopSpeechAt` functionbefore the Speech Synthesis Manager finishes processing input text,then the function might return before some input text has yet tobe spoken. Thus, before disposing of the text buffer, your applicationshould wait until its text-done callback function has been called(if one has been defined), or until it can determine (by, for exampleobtaining a speech status information structure) that the SpeechSynthesis Manager is no longer processing input text.

If the end of the input text buffer is reached before thespecified stopping point, the speech synthesizer stops at the endof the buffer without generating an error.

## See Also

### Starting, Stopping, and Pausing Speech

func ContinueSpeech(SpeechChannel) -> OSErr

Resumes speech paused by the `PauseSpeechAt` function.

Deprecated

func PauseSpeechAt(SpeechChannel, Int32) -> OSErr

Pauses speech on a speech channel.

Deprecated

func SpeakCFString(SpeechChannel, CFString, CFDictionary?) -> OSErr

Begins speaking a string represented as a `CFString` object.

Deprecated

func StopSpeech(SpeechChannel) -> OSErr

Terminates speech immediately on the specified channel.

Deprecated

