

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soTextDoneCallBack 

Global Variable

# soTextDoneCallBack

macOS 10.0+

``` source
var soTextDoneCallBack: OSType { get }
```

## Discussion

Set the callback function to be called whenthe Speech Synthesis Manager has finished processing speech beinggenerated on the speech channel. The `speechInfo` parameteris a pointer to an application-defined text-done callback function,whose syntax is described in SpeechTextDoneProcPtr. Passing `NULL` in `speechInfo` disablesthe text-done callback function.

This selector works with the `SetSpeechInfo` function.

