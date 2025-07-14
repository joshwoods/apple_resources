

- SensorKit
- SRSpeechMetrics
-  speechRecognition 

Instance Property

# speechRecognition

The partial or final results of the speech recognition request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var speechRecognition: SFSpeechRecognitionResult? { get }
```

## See Also

### Getting speech metrics and analytics

var audioLevel: SRAudioLevel?

The audio level of the speech.

class SRAudioLevel

An object that represents the audio level for a range of speech.

var soundClassification: SNClassificationResult?

The highest-ranking classifications in the time range.

var speechExpression: SRSpeechExpression?

The metrics and voice analytics for the range of speech.

