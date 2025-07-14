

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soWordCallBack 

Global Variable

# soWordCallBack

macOS 10.0+

``` source
var soWordCallBack: OSType { get }
```

## Discussion

Set the callback function to be called everytime the Speech Synthesis Manager is about to generate a word onthe speech channel. The `speechInfo` parameteris a pointer to an application-defined word callback function, whose syntax is described in SpeechWordProcPtr.Passing `NULL` in `speechInfo` disablesthe word callback function.

This selector works with the `SetSpeechInfo` function.

