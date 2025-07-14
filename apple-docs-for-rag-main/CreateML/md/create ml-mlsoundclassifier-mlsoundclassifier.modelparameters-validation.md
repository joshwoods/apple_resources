

- Create ML
- MLSoundClassifier
- MLSoundClassifier.ModelParameters
-  validation 

Instance Property

# validation

The sound classifier’s validation dataset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
var validation: MLSoundClassifier.ModelParameters.ValidationData
```

## See Also

### Accessing the training parameters

var maxIterations: Int

The largest number of iterations the training session can use.

var overlapFactor: Double

The proportion of overlap that the training session uses to analyze two consecutive windows in the audio data.

var algorithm: MLSoundClassifier.ModelParameters.ModelAlgorithmType

The algorithm the training session uses to train the sound classifier.

var featureExtractionTimeWindowSize: TimeInterval

A time duration, in seconds, the training session uses for each audio sample it reads from an audio file in a dataset.

