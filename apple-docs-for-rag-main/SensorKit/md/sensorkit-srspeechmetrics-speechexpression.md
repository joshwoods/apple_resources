

- SensorKit
- SRSpeechMetrics
-  speechExpression 

Instance Property

# speechExpression

The metrics and voice analytics for the range of speech.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var speechExpression: SRSpeechExpression? { get }
```

## See Also

### Getting speech metrics and analytics

var audioLevel: SRAudioLevel?

The audio level of the speech.

class SRAudioLevel

An object that represents the audio level for a range of speech.

var speechRecognition: SFSpeechRecognitionResult?

The partial or final results of the speech recognition request.

var soundClassification: SNClassificationResult?

The highest-ranking classifications in the time range.

