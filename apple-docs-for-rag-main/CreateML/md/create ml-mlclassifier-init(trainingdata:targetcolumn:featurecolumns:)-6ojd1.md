

- Create ML
- MLClassifier
-  init(trainingData:targetColumn:featureColumns:) 

Initializer

# init(trainingData:targetColumn:featureColumns:)

Creates a classifier.

macOS 12.0+

``` source
init(
    trainingData: DataFrame,
    targetColumn: String,
    featureColumns: [String]? = nil
) throws
```

## Parameters 

`trainingData`  

The training data

`targetColumn`  

Name of the column containing the class labels

`featureColumns`  

Names of the columns containing feature values. If `nil` all columns, other than the target column, will be used as feature values.

## See Also

### Creating and training a classifier

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?) throws

Creates a classifier from the feature columns in the training data to predict the categories in the target column.

Deprecated

var targetColumn: String

The name of the column you selected at initialization to define which categories the classifier predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the classifier.

