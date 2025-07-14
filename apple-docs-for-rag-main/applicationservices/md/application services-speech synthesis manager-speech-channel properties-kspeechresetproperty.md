

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechResetProperty 

Global Variable

# kSpeechResetProperty

Set a speech channel back to its default state.

macOS 10.5+

``` source
let kSpeechResetProperty: CFString
```

## Discussion

You can use this function to, for example, set speech pitch and speech rate to default values. There is no value associated with this property; to reset the channel to its default state, set the string to `NULL`.

This property works with the SetSpeechProperty(_:_:_:) function.

