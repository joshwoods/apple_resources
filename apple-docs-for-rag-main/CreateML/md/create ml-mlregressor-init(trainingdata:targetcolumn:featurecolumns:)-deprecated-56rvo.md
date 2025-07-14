

- Create ML
- MLRegressor
-  init(trainingData:targetColumn:featureColumns:) Deprecated

Initializer

# init(trainingData:targetColumn:featureColumns:)

Creates a regressor from the feature columns in the training data to predict the values in the target column.

macOS 10.14–13.0Deprecated

``` source
init(
    trainingData: MLDataTable,
    targetColumn: String,
    featureColumns: [String]? = nil
) throws
```

Deprecated

Use DataFrame instead of MLDataTable when initializing.

## Parameters 

`trainingData`  

A data table of training examples.

`targetColumn`  

The column name for the values in the training data the regressor should predict.

`featureColumns`  

The column names for the values in the training data that the regressor uses to predict the target value.

## Discussion

To view details about the supporting model picked by the MLRegressor, print the model’s description:

```
print(model)
```

## See Also

### Creating and training a regressor

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?) throws

Creates a regressor.

var targetColumn: String

The name of the column you selected at initialization to define which feature the regressor predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the regressor.

