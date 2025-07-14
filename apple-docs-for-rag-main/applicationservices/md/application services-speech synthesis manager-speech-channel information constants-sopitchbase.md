

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soPitchBase 

Global Variable

# soPitchBase

macOS 10.0+

``` source
var soPitchBase: OSType { get }
```

## Discussion

Get or set the speech channel’s baselinespeech pitch. This selector is intended for use by the Speech SynthesisManager; ordinarily, an application uses the GetSpeechPitch(_:_:) and SetSpeechPitch(_:_:) functions.The `speechInfo` parameteris a pointer to a variable of type `Fixed`.

This selector works with both the `GetSpeechInfo` and `SetSpeechInfo` functions.

Note

The change in speech pitch may not be noticeable until the next sentence or paragraph is spoken.

