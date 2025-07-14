

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soPhonemeCallBack 

Global Variable

# soPhonemeCallBack

macOS 10.0+

``` source
var soPhonemeCallBack: OSType { get }
```

## Discussion

Set the callback function to be called everytime the Speech Synthesis Manager is about to generate a phonemeon the speech channel. The `speechInfo` parameteris a pointer to an application-defined phoneme callback function,whose syntax is described in SpeechPhonemeProcPtr. Passing `NULL` in `speechInfo` disablesthe phoneme callback function.

This selector works with the `SetSpeechInfo` function.

