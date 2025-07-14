

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechSynthesizerInfoProperty 

Global Variable

# kSpeechSynthesizerInfoProperty

Get information about the speech synthesizer being used on the specified speech channel.

macOS 10.5+

``` source
let kSpeechSynthesizerInfoProperty: CFString
```

## Discussion

The value associated with this property is a `CFDictionary` object that contains information about the speech synthesizer being used on the specified speech channel. See Speech Synthesizer Information Keys for a description of the keys present in the dictionary.

This property works with the CopySpeechProperty(_:_:_:) function.

