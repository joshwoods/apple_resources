

- Application Services
- Speech Synthesis Manager
-  StopSpeech(\_:) Deprecated

Function

# StopSpeech(\_:)

Terminates speech immediately on the specified channel.

macOS 10.0–13.0Deprecated

``` source
func StopSpeech(_ chan: SpeechChannel) -> OSErr
```

## Parameters 

`chan`  

The speech channel on which speech is to be stopped.

## Return Value

A resultcode. See Result Codes.

## Discussion

The `StopSpeech` functionimmediately terminates speech on the channel specified by the `chan` parameter.After returning from `StopSpeech`,your application can safely release any text buffer that the speechsynthesizer has been using. You can call `StopSpeech` foran already idle channel without ill effect.

You can also stop speech by passing a zero-length string (or,in C, a `null` pointer)to one of the `SpeakString`, `SpeakText`,or `SpeakBuffer` functions.Doing this stops speech only in the specified speech channel (or,in the case of `SpeakString`,in the speech channel managed internally by the Speech SynthesisManager).

Before calling the `StopSpeech` function,you can use the `SpeechBusy` function,which is described in SpeechBusy(),to determine if a synthesizer is still speaking. If you are working withmultiple speech channels, you can use the status selector with thefunction `GetSpeechInfo` whichis described in GetSpeechInfo,to determine if a specific channel is still speaking.

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

func StopSpeechAt(SpeechChannel, Int32) -> OSErr

Terminates speech delivery on a specified channel eitherimmediately or at the end of the current word or sentence.

Deprecated

