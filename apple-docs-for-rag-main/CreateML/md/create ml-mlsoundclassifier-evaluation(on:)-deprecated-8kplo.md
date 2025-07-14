

- Create ML
- MLSoundClassifier
-  evaluation(on:) Deprecated

Instance Method

# evaluation(on:)

Generates metrics by evaluating the sound classifier’s performance on a dataset represented by a dictionary.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.15–11.0DeprecatedvisionOS 1.0+

``` source
func evaluation(on testingData: [String : [URL]]) -> MLClassifierMetrics
```

Deprecated

Use DataSource.filesByLabel to provide dictionary testing data instead.

## Parameters 

`testingData`  

A collection of labeled audio files represented by a dictionary. Each key of the dictionary is a label, and its value is an array of audio-file URLs.

## Return Value

An MLClassifierMetrics instance that contains the evaluation results.

## See Also

### Evaluating a sound classifier

func evaluation(on: MLSoundClassifier.DataSource) -> MLClassifierMetrics

Generates metrics by evaluating the sound classifier’s performance on a dataset represented by a data source.

