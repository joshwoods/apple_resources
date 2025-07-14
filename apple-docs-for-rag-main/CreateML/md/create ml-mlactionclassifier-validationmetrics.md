

- Create ML
- MLActionClassifier
-  validationMetrics 

Instance Property

# validationMetrics

Measurements of the action classifier’s performance on the validation dataset.

macOS 11.0+

``` source
var validationMetrics: MLClassifierMetrics { get }
```

## See Also

### Evaluating an action classifier

var trainingMetrics: MLClassifierMetrics

Measurements of the action classifier’s performance on the training dataset.

func evaluation(on: MLActionClassifier.DataSource) throws -> MLClassifierMetrics

Generates metrics describing the action classifier’s performance on labeled videos represented by a data source.

