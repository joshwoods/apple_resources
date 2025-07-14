

- Create ML
- MLClassifier
-  init(trainingData:targetColumn:featureColumns:) Deprecated

Initializer

# init(trainingData:targetColumn:featureColumns:)

Creates a classifier from the feature columns in the training data to predict the categories in the target column.

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

The column name for the values in the training data that the classifier should predict.

`featureColumns`  

The column names for the values in the training data that the classifier uses to predict the target value.

## Discussion

To view details about the supporting model chosen by the MLClassifier, print the model’s description:

```
print(model)
```

## See Also

### Creating and training a classifier

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?) throws

Creates a classifier.

var targetColumn: String

The name of the column you selected at initialization to define which categories the classifier predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the classifier.

