

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soSpeechDoneCallBack 

Global Variable

# soSpeechDoneCallBack

macOS 10.0+

``` source
var soSpeechDoneCallBack: OSType { get }
```

## Discussion

Set the callback function to be called whenthe Speech Synthesis Manager has finished generating speech on thespeech channel. The `speechInfo` parameteris a pointer to an application-defined speech-done callback function,whose syntax is described in SpeechDoneProcPtr.Passing `NULL` in `speechInfo` disablesthe speech-done callback function.

This selector works with the `SetSpeechInfo` function.

