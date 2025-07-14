

- Create ML
- MLImageClassifier
- 
  - MLImageClassifier
- MLImageClassifier.ModelParameters
- MLImageClassifier.ModelParameters.ValidationData
-  MLImageClassifier.ModelParameters.ValidationData.dictionary(\_:) Deprecated

Case

# MLImageClassifier.ModelParameters.ValidationData.dictionary(\_:)

A validation dataset represented by a dictionary.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.15–11.0DeprecatedvisionOS 1.0+

``` source
case dictionary([String : [URL]])
```

Deprecated

Use DataSource.filesByLabel to provide dictionary validation data instead.

## See Also

### Designating validation data

case split(strategy: MLSplitStrategy)

A validation dataset derived by randomly selecting a portion of the image classifier’s training dataset using the split strategy.

case dataSource(MLImageClassifier.DataSource)

A validation dataset represented by a data source.

case none

An empty validation dataset that skips the model validation phase after training.

