

- Create ML
- MLImageClassifier
-  evaluation(on:) 

Instance Method

# evaluation(on:)

Generates metrics describing the image classifier’s performance on labeled images represented by a data source.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
func evaluation(on labeledImages: MLImageClassifier.DataSource) -> MLClassifierMetrics
```

## Parameters 

`labeledImages`  

A set of labeled images in a data source.

## Return Value

The metrics that indicate the performance of the classifier when operating on the input dataset.

## Mentioned in 

Creating an Image Classifier Model

## See Also

### Evaluating an image classifier

func evaluation(on: [String : [URL]]) -> MLClassifierMetrics

Generates metrics describing the image classifier’s performance on labeled images represented by a dictionary.

Deprecated

