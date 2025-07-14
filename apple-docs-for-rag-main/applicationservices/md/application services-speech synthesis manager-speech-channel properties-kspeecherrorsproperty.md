

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechErrorsProperty 

Global Variable

# kSpeechErrorsProperty

Get speech-error information for the speech channel.

macOS 10.5+

``` source
let kSpeechErrorsProperty: CFString
```

## Discussion

The value associated with this property is a `CFDictionary` object that contains speech-error information. See Speech Error Keys for a description of the keys present in the dictionary.

This property lets you get information about various run-time errors that occur during speaking, such as the detection of badly formed embedded commands. Errors returned directly by the Speech Synthesis Manager are not reported here. If your application defines an error callback function, the function can use this property to get error information.

This property works with the CopySpeechProperty(_:_:_:) function.

