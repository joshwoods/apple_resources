

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechOutputToFileURLProperty 

Global Variable

# kSpeechOutputToFileURLProperty

Set the speech output destination to a file or to the computer’s speakers.

macOS 10.5+

``` source
let kSpeechOutputToFileURLProperty: CFString
```

## Discussion

The value associated with this property is a `CFURL` object. To write the speech output to a file, use the file’s `CFURLRef`; to generate the sound through the computer’s speakers, use `NULL`.

This property works with the SetSpeechProperty(_:_:_:) function.

