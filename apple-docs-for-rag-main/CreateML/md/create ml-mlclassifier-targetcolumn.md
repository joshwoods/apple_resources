

- Create ML
- MLClassifier
-  targetColumn 

Instance Property

# targetColumn

The name of the column you selected at initialization to define which categories the classifier predicts.

macOS 10.14+

``` source
var targetColumn: String { get }
```

## See Also

### Creating and training a classifier

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?) throws

Creates a classifier.

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?) throws

Creates a classifier from the feature columns in the training data to predict the categories in the target column.

Deprecated

var featureColumns: [String]

The names of the columns you selected at initialization to train the classifier.

