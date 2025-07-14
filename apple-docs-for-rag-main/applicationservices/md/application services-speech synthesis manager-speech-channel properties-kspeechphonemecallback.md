

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechPhonemeCallBack 

Global Variable

# kSpeechPhonemeCallBack

Set the callback function to be called every time the Speech Synthesis Manager is about to generate a phoneme on the speech channel.

macOS 10.5+

``` source
let kSpeechPhonemeCallBack: CFString
```

## Discussion

The value associated with this property is `CFNumber` object whose value is a pointer to an application-defined phoneme callback function, whose syntax is described in SpeechPhonemeProcPtr. Passing a `CFNumber` object that contains the value `NULL` for the value of this property disables the phoneme callback function.

This property works with the SetSpeechProperty(_:_:_:) function.

