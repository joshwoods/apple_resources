

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechWordCFCallBack 

Global Variable

# kSpeechWordCFCallBack

Set the callback function to be called every time the Speech Synthesis Manager is about to generate a word on the speech channel.

macOS 10.5+

``` source
let kSpeechWordCFCallBack: CFString
```

## Discussion

The value associated with this property is `CFNumber` object whose value is a pointer to an application-defined word callback function, whose syntax is described in SpeechWordCFProcPtr. Passing a `CFNumber` object that contains the value `NULL` for the value of this property disables the word callback function.

This property works with the SetSpeechProperty(_:_:_:) function.

