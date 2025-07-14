

- Create ML
- MLHandActionClassifier
-  trainingMetrics 

Instance Property

# trainingMetrics

Measurements of the hand action classifier’s performance on the training dataset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
var trainingMetrics: MLClassifierMetrics
```

## See Also

### Evaluating a hand action classifier

var validationMetrics: MLClassifierMetrics

Measurements of the hand action classifier’s performance on the validation dataset.

func evaluation(on: MLHandActionClassifier.DataSource) throws -> MLClassifierMetrics

Generates metrics describing the hand action classifier’s performance on labeled videos.

