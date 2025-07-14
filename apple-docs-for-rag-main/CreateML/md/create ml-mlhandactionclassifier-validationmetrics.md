

- Create ML
- MLHandActionClassifier
-  validationMetrics 

Instance Property

# validationMetrics

Measurements of the hand action classifier’s performance on the validation dataset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
var validationMetrics: MLClassifierMetrics
```

## See Also

### Evaluating a hand action classifier

var trainingMetrics: MLClassifierMetrics

Measurements of the hand action classifier’s performance on the training dataset.

func evaluation(on: MLHandActionClassifier.DataSource) throws -> MLClassifierMetrics

Generates metrics describing the hand action classifier’s performance on labeled videos.

