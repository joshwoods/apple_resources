

- Speech
- SFSpeechRecognitionRequest
-  shouldReportPartialResults 

Instance Property

# shouldReportPartialResults

A Boolean value that indicates whether you want intermediate results returned for each utterance.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var shouldReportPartialResults: Bool { get set }
```

## Discussion

The default value of this property is `true`. If you want only final results (and you don’t care about intermediate results), set this property to `false` to prevent the system from doing extra work.

## See Also

### Recognition Request Configuration

var requiresOnDeviceRecognition: Bool

A Boolean value that determines whether a request must keep its audio data on the device.

var contextualStrings: [String]

An array of phrases that should be recognized, even if they are not in the system vocabulary.

