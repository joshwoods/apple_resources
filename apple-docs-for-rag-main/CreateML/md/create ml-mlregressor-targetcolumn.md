

- Create ML
- MLRegressor
-  targetColumn 

Instance Property

# targetColumn

The name of the column you selected at initialization to define which feature the regressor predicts.

macOS 10.14+

``` source
var targetColumn: String { get }
```

## See Also

### Creating and training a regressor

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?) throws

Creates a regressor.

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?) throws

Creates a regressor from the feature columns in the training data to predict the values in the target column.

Deprecated

var featureColumns: [String]

The names of the columns you selected at initialization to train the regressor.

