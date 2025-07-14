

- Create ML
- MLHandPoseClassifier
-  validationMetrics 

Instance Property

# validationMetrics

Measurements of the hand pose classifier’s performance on the validation dataset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
var validationMetrics: MLClassifierMetrics
```

## See Also

### Evaluating a hand pose classifier

var trainingMetrics: MLClassifierMetrics

Measurements of the hand pose classifier’s performance on the training dataset.

func evaluation(on: MLHandPoseClassifier.DataSource) throws -> MLClassifierMetrics

Generates metrics that describe the hand pose classifier’s performance with a dataset of labeled images.

