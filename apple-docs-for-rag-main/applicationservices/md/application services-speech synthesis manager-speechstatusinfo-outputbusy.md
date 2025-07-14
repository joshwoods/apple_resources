

- Application Services
- Speech Synthesis Manager
- SpeechStatusInfo
-  outputBusy 

Instance Property

# outputBusy

Whether the speech channel is currently producing speech. A speech channel is considered to be producing speech even at some times when no audio data is being produced through the Macintosh speaker. This occurs, for example, when the Speech Synthesis Manager is processing an input buffer but has not yet initiated speech or when speech output is paused.

macOS 10.0+

``` source
var outputBusy: DarwinBoolean
```

