

- Create ML
- MLImageClassifier
-  evaluation(on:) Deprecated

Instance Method

# evaluation(on:)

Generates metrics describing the image classifier’s performance on labeled images represented by a dictionary.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–11.0DeprecatedvisionOS 1.0+

``` source
func evaluation(on labeledImages: [String : [URL]]) -> MLClassifierMetrics
```

Deprecated

Use DataSource.filesByLabel to provide dictionary training data instead.

## Parameters 

`labeledImages`  

A dictionary with keys that are labels, and values that are arrays of image URLs corresponding to those labels.

## Return Value

The metrics that indicate the performance of the classifier when operating on the input dataset.

## See Also

### Evaluating an image classifier

func evaluation(on: MLImageClassifier.DataSource) -> MLClassifierMetrics

Generates metrics describing the image classifier’s performance on labeled images represented by a data source.

