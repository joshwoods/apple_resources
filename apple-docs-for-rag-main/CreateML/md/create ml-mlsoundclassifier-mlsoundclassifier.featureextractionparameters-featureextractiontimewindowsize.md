

- Create ML
- MLSoundClassifier
- MLSoundClassifier.FeatureExtractionParameters
-  featureExtractionTimeWindowSize 

Instance Property

# featureExtractionTimeWindowSize

A time duration, in seconds, that determines how much audio data the feature-extraction session reads each time it samples an audio file.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
var featureExtractionTimeWindowSize: TimeInterval { get set }
```

## Discussion

The time-window size defaults to `0.975` seconds and must be in the range `[0.5, 15.0]`.

Feature-extraction sessions that use MLSoundClassifier.ModelParameters.FeatureExtractorType.vggish(revision:) ignore this value and always use a time-window size of `0.975` seconds.

## See Also

### Accessing feature extraction parameters

var overlapFactor: Double

The proportion of overlap that the feature-extraction session uses to analyze two consecutive windows in the audio data.

var featureExtractor: MLSoundClassifier.ModelParameters.FeatureExtractorType

The algorithm type the session uses to extract features from audio files.

