

- Create ML
- MLActionClassifier
-  evaluation(on:) 

Instance Method

# evaluation(on:)

Generates metrics describing the action classifier’s performance on labeled videos represented by a data source.

macOS 11.0+

``` source
func evaluation(on annotatedVideos: MLActionClassifier.DataSource) throws -> MLClassifierMetrics
```

## Discussion

- annotatedVideos: A collection of labeled videos represented by a data source.

## See Also

### Evaluating an action classifier

var trainingMetrics: MLClassifierMetrics

Measurements of the action classifier’s performance on the training dataset.

var validationMetrics: MLClassifierMetrics

Measurements of the action classifier’s performance on the validation dataset.

