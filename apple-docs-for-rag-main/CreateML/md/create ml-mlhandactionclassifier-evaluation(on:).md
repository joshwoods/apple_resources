

- Create ML
- MLHandActionClassifier
-  evaluation(on:) 

Instance Method

# evaluation(on:)

Generates metrics describing the hand action classifier’s performance on labeled videos.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
func evaluation(on annotatedVideos: MLHandActionClassifier.DataSource) throws -> MLClassifierMetrics
```

## Discussion

- annotatedVideos : An MLHandActionClassifier.DataSource instance.

## See Also

### Evaluating a hand action classifier

var trainingMetrics: MLClassifierMetrics

Measurements of the hand action classifier’s performance on the training dataset.

var validationMetrics: MLClassifierMetrics

Measurements of the hand action classifier’s performance on the validation dataset.

