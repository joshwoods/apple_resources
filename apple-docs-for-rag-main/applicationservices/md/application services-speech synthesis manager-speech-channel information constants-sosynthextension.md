

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soSynthExtension 

Global Variable

# soSynthExtension

macOS 10.0+

``` source
var soSynthExtension: OSType { get }
```

## Discussion

Get or set synthesizer-specific informationor settings. The `speechInfo` parameteris a pointer to a speech extension data structure, described in SpeechXtndData. Yourapplication should set the `synthCreator` fieldof this structure before calling `GetSpeechInfo` or `SetSpeechInfo`.Ordinarily, your application must pass additional information tothe synthesizer in the `synthData` field.

This selector works with both the `GetSpeechInfo` and `SetSpeechInfo` functions.

