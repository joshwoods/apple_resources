

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechOutputToExtAudioFileProperty 

Global Variable

# kSpeechOutputToExtAudioFileProperty

Set the speech output destination to an extended audio file or to the computer’s speakers.

macOS 10.6+

``` source
let kSpeechOutputToExtAudioFileProperty: CFString
```

## Discussion

The value associated with this property is a `CFNumber` object whose value is an `ExtAudioFileRef`. To write the speech output to an extended audio file, use the file’s ExtAudioFileRef; to generate sound through the computer’s speakers, use `NULL`.

This property works with the SetSpeechProperty(_:_:_:) function.

