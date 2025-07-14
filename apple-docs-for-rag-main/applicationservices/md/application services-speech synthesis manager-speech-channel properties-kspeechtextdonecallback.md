

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechTextDoneCallBack 

Global Variable

# kSpeechTextDoneCallBack

Set the callback function to be called when the Speech Synthesis Manager has finished processing speech being generated on the speech channel.

macOS 10.5+

``` source
let kSpeechTextDoneCallBack: CFString
```

## Discussion

The value associated with this property is a `CFNumber` object whose value is a pointer to an application-defined text-done callback function, whose syntax is described in SpeechTextDoneProcPtr. Passing a `CFNumber` object that contains the value `NULL` disables the text-done callback function.

This property works with the SetSpeechProperty(_:_:_:) function.

