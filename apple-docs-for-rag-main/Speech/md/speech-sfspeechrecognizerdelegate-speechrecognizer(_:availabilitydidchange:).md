

- Speech
- SFSpeechRecognizerDelegate
-  speechRecognizer(\_:availabilityDidChange:) 

Instance Method

# speechRecognizer(\_:availabilityDidChange:)

Tells the delegate that the availability of its associated speech recognizer changed.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
optional func speechRecognizer(
    _ speechRecognizer: SFSpeechRecognizer,
    availabilityDidChange available: Bool
)
```

## Parameters 

`speechRecognizer`  

The SFSpeechRecognizer object whose availability changed.

`available`  

A Boolean value that indicates the new availability of the speech recognizer.

