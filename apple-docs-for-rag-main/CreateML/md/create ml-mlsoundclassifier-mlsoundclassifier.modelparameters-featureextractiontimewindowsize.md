

- Create ML
- MLSoundClassifier
- MLSoundClassifier.ModelParameters
-  featureExtractionTimeWindowSize 

Instance Property

# featureExtractionTimeWindowSize

A time duration, in seconds, the training session uses for each audio sample it reads from an audio file in a dataset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
var featureExtractionTimeWindowSize: TimeInterval { get set }
```

## Discussion

The time-window size value defaults to `0.975` seconds and must be in the range `[0.5, 15.0]`.

Training sessions that use MLSoundClassifier.ModelParameters.FeatureExtractorType.vggish(revision:) ignore this value and always use a time-window size of `0.975` seconds.

## See Also

### Accessing the training parameters

var validation: MLSoundClassifier.ModelParameters.ValidationData

The sound classifier’s validation dataset.

var maxIterations: Int

The largest number of iterations the training session can use.

var overlapFactor: Double

The proportion of overlap that the training session uses to analyze two consecutive windows in the audio data.

var algorithm: MLSoundClassifier.ModelParameters.ModelAlgorithmType

The algorithm the training session uses to train the sound classifier.

