

- Create ML
- MLSoundClassifier
-  evaluation(on:) 

Instance Method

# evaluation(on:)

Generates metrics by evaluating the sound classifier’s performance on a dataset represented by a data source.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
func evaluation(on testingData: MLSoundClassifier.DataSource) -> MLClassifierMetrics
```

## Parameters 

`testingData`  

A collection of labeled audio files represented by an MLSoundClassifier.DataSource.

## Return Value

An MLClassifierMetrics instance that contains the evaluation results.

## See Also

### Evaluating a sound classifier

func evaluation(on: [String : [URL]]) -> MLClassifierMetrics

Generates metrics by evaluating the sound classifier’s performance on a dataset represented by a dictionary.

Deprecated

