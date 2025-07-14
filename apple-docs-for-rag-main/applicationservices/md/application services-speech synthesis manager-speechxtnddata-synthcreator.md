

- Application Services
- Speech Synthesis Manager
- SpeechXtndData
-  synthCreator 

Instance Property

# synthCreator

The synthesizer’s creator ID, identical to the value stored in the `synthManufacturer` field of a speech version information structure. You should set this field to the appropriate value before calling `GetSpeechInfo` or `SetSpeechInfo`.

macOS 10.0+

``` source
var synthCreator: OSType
```

