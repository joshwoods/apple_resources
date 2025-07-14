

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechSpeechDoneCallBack 

Global Variable

# kSpeechSpeechDoneCallBack

Set the callback function to be called when the Speech Synthesis Manager has finished generating speech on the speech channel.

macOS 10.5+

``` source
let kSpeechSpeechDoneCallBack: CFString
```

## Discussion

The value associated with this property is `CFNumber` object whose value is a pointer to an application-defined speech-done callback function, whose syntax is described in SpeechDoneProcPtr. Passing `NULL` for the value of this property disables the speech-done callback function.

This property works with the SetSpeechProperty(_:_:_:) function.

