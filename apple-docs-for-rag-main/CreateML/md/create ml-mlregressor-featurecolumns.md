

- Create ML
- MLRegressor
-  featureColumns 

Instance Property

# featureColumns

The names of the columns you selected at initialization to train the regressor.

macOS 10.14+

``` source
var featureColumns: [String] { get }
```

## See Also

### Creating and training a regressor

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?) throws

Creates a regressor.

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?) throws

Creates a regressor from the feature columns in the training data to predict the values in the target column.

Deprecated

var targetColumn: String

The name of the column you selected at initialization to define which feature the regressor predicts.

