

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechCurrentVoiceProperty 

Global Variable

# kSpeechCurrentVoiceProperty

Set the current voice on the current speech channel to the specified voice.

macOS 10.5+

``` source
let kSpeechCurrentVoiceProperty: CFString
```

## Discussion

The value associated with this property is a `CFDictionary` object that contains the phoneme symbols and example words defined for the current synthesizer. Your application might use this information to show the user what symbols to use when entering phonemic text directly. See Phoneme Symbols Keys for the keys you can use to specify values in this dictionary.

This property works with the SetSpeechProperty(_:_:_:) function.

