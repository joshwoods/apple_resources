

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soReset 

Global Variable

# soReset

macOS 10.0+

``` source
var soReset: OSType { get }
```

## Discussion

Set a speech channel back to its default state.For example, speech pitch and speech rate are set to default values.The `speechInfo` parametershould be set to `NULL`.

This selector works with the `SetSpeechInfo` function.

