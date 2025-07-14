

- Create ML
- MLSoundClassifier
- MLSoundClassifier.FeatureExtractionParameters
-  featureExtractor 

Instance Property

# featureExtractor

The algorithm type the session uses to extract features from audio files.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
var featureExtractor: MLSoundClassifier.ModelParameters.FeatureExtractorType
```

## See Also

### Accessing feature extraction parameters

var overlapFactor: Double

The proportion of overlap that the feature-extraction session uses to analyze two consecutive windows in the audio data.

var featureExtractionTimeWindowSize: TimeInterval

A time duration, in seconds, that determines how much audio data the feature-extraction session reads each time it samples an audio file.

