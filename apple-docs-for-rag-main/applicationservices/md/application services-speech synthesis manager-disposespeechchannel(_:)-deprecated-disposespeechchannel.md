

- Application Services
- Speech Synthesis Manager
-  DisposeSpeechChannel(\_:) Deprecated

Function

# DisposeSpeechChannel(\_:)

Disposes of an existing speech channel.

macOS 10.0–13.0Deprecated

``` source
func DisposeSpeechChannel(_ chan: SpeechChannel) -> OSErr
```

## Parameters 

`chan`  

The speech channel to dispose of.

## Return Value

A resultcode. See Result Codes.

## Discussion

The `DisposeSpeechChannel` functiondisposes of the speech channel specified in the `chan` parameterand releases all memory the channel occupies. If the speech channelspecified is producing speech, then the `DisposeSpeechChannel` functionimmediately stops speech before disposing of the channel. If youhave defined a text-done callback function or a speech-done callbackfunction, the function will not be called before the channel is disposedof.

The Speech Synthesis Manager releases any speech channelsthat have not been explicitly disposed of by an application whenthe application quits. In general, however, your application shoulddispose of any speech channels it has created whenever it receivesa suspend event. This ensures that other applications can take fulladvantage of Speech Synthesis Manager and Sound Manager capabilities.

## See Also

### Managing Speech Channels

func NewSpeechChannel(UnsafeMutablePointer&lt;VoiceSpec>?, UnsafeMutablePointer&lt;SpeechChannel?>) -> OSErr

Creates a new speech channel.

Deprecated

