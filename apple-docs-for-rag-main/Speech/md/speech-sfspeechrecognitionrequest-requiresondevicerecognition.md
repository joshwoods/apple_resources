

- Speech
- SFSpeechRecognitionRequest
-  requiresOnDeviceRecognition 

Instance Property

# requiresOnDeviceRecognition

A Boolean value that determines whether a request must keep its audio data on the device.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
var requiresOnDeviceRecognition: Bool { get set }
```

## Discussion

Set this property to true to prevent an SFSpeechRecognitionRequest from sending audio over the network. However, on-device requests won’t be as accurate.

Note

The request only honors this setting if the supportsOnDeviceRecognition (SFSpeechRecognizer) property is also true.

## See Also

### Recognition Request Configuration

var shouldReportPartialResults: Bool

A Boolean value that indicates whether you want intermediate results returned for each utterance.

var contextualStrings: [String]

An array of phrases that should be recognized, even if they are not in the system vocabulary.

