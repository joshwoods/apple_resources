

- Create ML
- MLSoundClassifier
- MLSoundClassifier.ModelParameters
- MLSoundClassifier.ModelParameters.ValidationData
-  MLSoundClassifier.ModelParameters.ValidationData.none 

Case

# MLSoundClassifier.ModelParameters.ValidationData.none

An empty validation dataset that skips the model validation phase after training.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
case none
```

## See Also

### Designating validation data

case split(strategy: MLSplitStrategy)

A validation dataset derived by randomly selecting a portion of the sound classifier’s training dataset using the split strategy.

case dataSource(MLSoundClassifier.DataSource)

A validation dataset represented by a data source.

case dictionary([String : [URL]])

A validation dataset represented by a dictionary.

Deprecated

