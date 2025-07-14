

- Create ML
- MLActionClassifier
-  trainingMetrics 

Instance Property

# trainingMetrics

Measurements of the action classifier’s performance on the training dataset.

macOS 11.0+

``` source
var trainingMetrics: MLClassifierMetrics { get }
```

## See Also

### Evaluating an action classifier

var validationMetrics: MLClassifierMetrics

Measurements of the action classifier’s performance on the validation dataset.

func evaluation(on: MLActionClassifier.DataSource) throws -> MLClassifierMetrics

Generates metrics describing the action classifier’s performance on labeled videos represented by a data source.

