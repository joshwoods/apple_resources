

- Speech
- SFSpeechRecognizer
-  supportsOnDeviceRecognition 

Instance Property

# supportsOnDeviceRecognition

A Boolean value that indicates whether the speech recognizer can operate without network access.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
var supportsOnDeviceRecognition: Bool { get set }
```

## Discussion

An SFSpeechRecognitionRequest can only honor its requiresOnDeviceRecognition property if supportsOnDeviceRecognition is true. If supportsOnDeviceRecognition is false, the SFSpeechRecognizer requires a network in order to recognize speech.

## See Also

### Monitoring the Availability of Speech Recognition

var delegate: (any SFSpeechRecognizerDelegate)?

The delegate object that handles changes to the availability of speech recognition services.

protocol SFSpeechRecognizerDelegate

A protocol that you adopt in your objects to track the availability of a speech recognizer.

var isAvailable: Bool

A Boolean value that indicates whether the speech recognizer is currently available.

