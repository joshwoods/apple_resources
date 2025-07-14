

- Create ML
- MLSoundClassifier
- MLSoundClassifier.ModelParameters
- MLSoundClassifier.ModelParameters.ValidationData
-  MLSoundClassifier.ModelParameters.ValidationData.split(strategy:) 

Case

# MLSoundClassifier.ModelParameters.ValidationData.split(strategy:)

A validation dataset derived by randomly selecting a portion of the sound classifier’s training dataset using the split strategy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
case split(strategy: MLSplitStrategy)
```

## Discussion

- strategy: The partition method this case uses to create the validation dataset from the training dataset.

## See Also

### Designating validation data

case dataSource(MLSoundClassifier.DataSource)

A validation dataset represented by a data source.

case dictionary([String : [URL]])

A validation dataset represented by a dictionary.

Deprecated

case none

An empty validation dataset that skips the model validation phase after training.

