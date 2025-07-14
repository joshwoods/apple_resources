

- Speech
- SFSpeechRecognizer
-  delegate 

Instance Property

# delegate

The delegate object that handles changes to the availability of speech recognition services.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
weak var delegate: (any SFSpeechRecognizerDelegate)? { get set }
```

## Discussion

Provide a delegate object when you want to monitor changes to the availability of speech recognition services. Your delegate object must conform to the SFSpeechRecognizerDelegate protocol.

## See Also

### Monitoring the Availability of Speech Recognition

protocol SFSpeechRecognizerDelegate

A protocol that you adopt in your objects to track the availability of a speech recognizer.

var isAvailable: Bool

A Boolean value that indicates whether the speech recognizer is currently available.

var supportsOnDeviceRecognition: Bool

A Boolean value that indicates whether the speech recognizer can operate without network access.

