

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechPhonemeOptionsProperty 

Global Variable

# kSpeechPhonemeOptionsProperty

Get or set the options for the generation of phonetic output.

macOS 10.6+

``` source
let kSpeechPhonemeOptionsProperty: CFString
```

## Discussion

The value associated with this property is a pointer to an `CFNumber` object containing the flags (options) you would pass to soPhonemeOptions. (See Phoneme Generation Options for a complete list of options.)

This property works with the SetSpeechProperty(_:_:_:) and the CopySpeechProperty(_:_:_:) functions.

