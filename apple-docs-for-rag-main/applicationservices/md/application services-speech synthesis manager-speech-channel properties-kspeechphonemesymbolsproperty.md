

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechPhonemeSymbolsProperty 

Global Variable

# kSpeechPhonemeSymbolsProperty

Get a list of phoneme symbols and example words defined for the speech channel’s synthesizer.

macOS 10.5+

``` source
let kSpeechPhonemeSymbolsProperty: CFString
```

## Discussion

The value associated with this property is a `CFDictionary` object that contains the phoneme symbols and example words defined for the current synthesizer. Your application might use this information to show the user what symbols to use when entering phonemic text directly. See Phoneme Symbols Keys for a description of the keys present in the dictionary.

This property works with the CopySpeechProperty(_:_:_:) function.

