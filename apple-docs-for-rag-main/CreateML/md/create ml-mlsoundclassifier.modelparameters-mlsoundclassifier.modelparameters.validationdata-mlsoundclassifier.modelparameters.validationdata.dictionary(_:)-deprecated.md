

- Create ML
- MLSoundClassifier
- 
  - MLSoundClassifier
- MLSoundClassifier.ModelParameters
- MLSoundClassifier.ModelParameters.ValidationData
-  MLSoundClassifier.ModelParameters.ValidationData.dictionary(\_:) Deprecated

Case

# MLSoundClassifier.ModelParameters.ValidationData.dictionary(\_:)

A validation dataset represented by a dictionary.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.15–11.0DeprecatedvisionOS 1.0+

``` source
case dictionary([String : [URL]])
```

Deprecated

Use DataSource.filesByLabel to provide dictionary validation data instead.

## Discussion

- dictionary: A validation dataset that uses a collection of labeled audio files represented by a dictionary. Each key of the dictionary is a label, and its value is an array of audio-file URLs.

## See Also

### Designating validation data

case split(strategy: MLSplitStrategy)

A validation dataset derived by randomly selecting a portion of the sound classifier’s training dataset using the split strategy.

case dataSource(MLSoundClassifier.DataSource)

A validation dataset represented by a data source.

case none

An empty validation dataset that skips the model validation phase after training.

