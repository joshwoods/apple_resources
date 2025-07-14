

- Speech
- SFSpeechRecognizer
-  isAvailable 

Instance Property

# isAvailable

A Boolean value that indicates whether the speech recognizer is currently available.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var isAvailable: Bool { get }
```

## Discussion

When the value of this property is true, you may create new speech recognition tasks. When value of this property is false, speech recognition services are not available.

## See Also

### Monitoring the Availability of Speech Recognition

var delegate: (any SFSpeechRecognizerDelegate)?

The delegate object that handles changes to the availability of speech recognition services.

protocol SFSpeechRecognizerDelegate

A protocol that you adopt in your objects to track the availability of a speech recognizer.

var supportsOnDeviceRecognition: Bool

A Boolean value that indicates whether the speech recognizer can operate without network access.

