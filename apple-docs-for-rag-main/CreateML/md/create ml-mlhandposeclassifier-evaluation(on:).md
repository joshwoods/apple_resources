

- Create ML
- MLHandPoseClassifier
-  evaluation(on:) 

Instance Method

# evaluation(on:)

Generates metrics that describe the hand pose classifier’s performance with a dataset of labeled images.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
func evaluation(on annotatedImages: MLHandPoseClassifier.DataSource) throws -> MLClassifierMetrics
```

## See Also

### Evaluating a hand pose classifier

var trainingMetrics: MLClassifierMetrics

Measurements of the hand pose classifier’s performance on the training dataset.

var validationMetrics: MLClassifierMetrics

Measurements of the hand pose classifier’s performance on the validation dataset.

