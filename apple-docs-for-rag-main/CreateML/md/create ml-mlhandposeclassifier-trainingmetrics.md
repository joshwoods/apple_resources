

- Create ML
- MLHandPoseClassifier
-  trainingMetrics 

Instance Property

# trainingMetrics

Measurements of the hand pose classifier’s performance on the training dataset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
var trainingMetrics: MLClassifierMetrics
```

## See Also

### Evaluating a hand pose classifier

var validationMetrics: MLClassifierMetrics

Measurements of the hand pose classifier’s performance on the validation dataset.

func evaluation(on: MLHandPoseClassifier.DataSource) throws -> MLClassifierMetrics

Generates metrics that describe the hand pose classifier’s performance with a dataset of labeled images.

