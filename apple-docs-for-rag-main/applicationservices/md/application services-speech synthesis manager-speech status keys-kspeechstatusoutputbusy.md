

- Application Services
- Speech Synthesis Manager
- Speech Status Keys
-  kSpeechStatusOutputBusy 

Global Variable

# kSpeechStatusOutputBusy

Indicates whether the speech channel is currently producing speech.

macOS 10.5+

``` source
let kSpeechStatusOutputBusy: CFString
```

## Discussion

A speech channel is considered to be producing speech even at some times when no audio data is being produced through the computer’s speaker. This occurs, for example, when the Speech Synthesis Manager is processing input, but has not yet initiated speech or when speech output is paused.

