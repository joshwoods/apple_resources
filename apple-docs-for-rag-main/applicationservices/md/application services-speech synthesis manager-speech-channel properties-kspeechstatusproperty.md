

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechStatusProperty 

Global Variable

# kSpeechStatusProperty

Get speech-status information for the speech channel.

macOS 10.5+

``` source
let kSpeechStatusProperty: CFString
```

## Discussion

The value associated with this property is a `CFDictionary` object that contains speech-status information for the speech channel. See Speech Status Keys for a description of the keys present in the dictionary.

This property works with the CopySpeechProperty(_:_:_:) function.

