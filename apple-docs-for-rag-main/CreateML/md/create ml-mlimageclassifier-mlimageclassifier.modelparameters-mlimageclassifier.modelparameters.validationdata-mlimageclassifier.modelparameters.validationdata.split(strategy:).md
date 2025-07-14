

- Create ML
- MLImageClassifier
- MLImageClassifier.ModelParameters
- MLImageClassifier.ModelParameters.ValidationData
-  MLImageClassifier.ModelParameters.ValidationData.split(strategy:) 

Case

# MLImageClassifier.ModelParameters.ValidationData.split(strategy:)

A validation dataset derived by randomly selecting a portion of the image classifier’s training dataset using the split strategy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
case split(strategy: MLSplitStrategy)
```

## See Also

### Designating validation data

case dataSource(MLImageClassifier.DataSource)

A validation dataset represented by a data source.

case dictionary([String : [URL]])

A validation dataset represented by a dictionary.

Deprecated

case none

An empty validation dataset that skips the model validation phase after training.

