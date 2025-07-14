

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soSyncCallBack 

Global Variable

# soSyncCallBack

macOS 10.0+

``` source
var soSyncCallBack: OSType { get }
```

## Discussion

Set the callback function to be called whenthe Speech Synthesis Manager encounters a synchronization commandwithin an embedded speech command in text being processed on thespeech channel. The `speechInfo` parameteris a pointer to an application-defined synchronization callback function,whose syntax is described in SpeechSyncProcPtr.Passing `NULL` in `speechInfo` disablesthe synchronization callback function.

This selector works with the `SetSpeechInfo` function.

