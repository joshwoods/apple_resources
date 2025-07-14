

- Create ML
- MLImageClassifier
- MLImageClassifier.ModelParameters
- MLImageClassifier.ModelParameters.ValidationData
-  MLImageClassifier.ModelParameters.ValidationData.dataSource(\_:) 

Case

# MLImageClassifier.ModelParameters.ValidationData.dataSource(\_:)

A validation dataset represented by a data source.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
case dataSource(MLImageClassifier.DataSource)
```

## See Also

### Designating validation data

case split(strategy: MLSplitStrategy)

A validation dataset derived by randomly selecting a portion of the image classifier’s training dataset using the split strategy.

case dictionary([String : [URL]])

A validation dataset represented by a dictionary.

Deprecated

case none

An empty validation dataset that skips the model validation phase after training.

