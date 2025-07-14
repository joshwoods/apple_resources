

- Application Services
- Speech Synthesis Manager
- Synthesizer Option Keys
-  kSpeechNoSpeechInterrupt 

Global Variable

# kSpeechNoSpeechInterrupt

Do not interrupt current speech.

macOS 10.5+

``` source
let kSpeechNoSpeechInterrupt: CFString
```

## Discussion

The `kSpeechNoSpeechInterrupt` key is used to control the behavior of SpeakCFString(_:_:_:) when it is called on a speech channel that is busy. When `kSpeechNoSpeechInterrupt` is not specified in the `options` dictionary (or if it is specified with the value `kCFBooleanFalse`), `SpeakCFString` immediately interrupts the speech currently being produced on the specified speech channel and the new `aString` text is spoken. When `kSpeechNoSpeechInterrupt` is specified with the value `kCFBooleanTrue`, the request to speak on a speech channel that is already busy causes the new `aString` text to be ignored and the `synthNotReady` error to be returned.

