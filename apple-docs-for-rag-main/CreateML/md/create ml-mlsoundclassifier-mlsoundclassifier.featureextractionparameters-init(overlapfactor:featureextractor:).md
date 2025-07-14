

- Create ML
- MLSoundClassifier
- MLSoundClassifier.FeatureExtractionParameters
-  init(overlapFactor:featureExtractor:) 

Initializer

# init(overlapFactor:featureExtractor:)

Creates the parameters for a feature-extraction session with a default time window size.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
init(
    overlapFactor: Double = __Defaults.overlapFactor,
    featureExtractor: MLSoundClassifier.ModelParameters.FeatureExtractorType = __Defaults.featureExtractor
)
```

## Parameters 

`overlapFactor`  

A portion of overlap between consecutive audio analysis windows. The value must be in the range `[0.0, 1.0)`.

`featureExtractor`  

An algorithm type the session uses to extract features from audio files.

## Discussion

The initializer sets featureExtractionTimeWindowSize to a default value.

## See Also

### Creating feature extraction parameters

init(overlapFactor: Double, featureExtractor: MLSoundClassifier.ModelParameters.FeatureExtractorType, featureExtractionTimeWindowSize: TimeInterval?)

Creates the parameters for a feature-extraction session.

