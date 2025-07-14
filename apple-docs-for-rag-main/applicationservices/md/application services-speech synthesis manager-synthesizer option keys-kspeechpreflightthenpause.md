

- Application Services
- Speech Synthesis Manager
- Synthesizer Option Keys
-  kSpeechPreflightThenPause 

Global Variable

# kSpeechPreflightThenPause

Compute speech without generating it.

macOS 10.5+

``` source
let kSpeechPreflightThenPause: CFString
```

## Discussion

The `kSpeechPreflightThenPause` key is used to minimize the latency experienced when the speech synthesizer is attempting to speak. To achieve this, specify the `kSpeechPreflightThenPause` key, with the value `kCFBooleanTrue`, in the `options` dictionary. This causes the speech synthesizer to process the input text as necessary to the point where it is ready to begin producing speech output. At this point, the synthesizer enters a paused state and returns to the caller. When the application is ready to produce speech, it should call ContinueSpeech(_:) to begin speaking.

If you do not specify the `kSpeechPreflightThenPause` key (or you specify it with the value `kCFBooleanFalse`), SpeakCFString(_:_:_:) starts speaking the input text after processing it.

