

- Create ML
- MLRandomForestClassifier
-  targetColumn 

Instance Property

# targetColumn

The name of the column you selected at initialization to define which categories the classifier predicts.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var targetColumn: String
```

## Discussion

Changing the value of this property doesn’t retrain the model or affect its behavior.

## See Also

### Creating and training a random forest classifier

init(checkpoint: MLCheckpoint) throws

Creates a random forest classifier classifier from a checkpoint.

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLRandomForestClassifier.ModelParameters) throws

Creates a random forest classifier.

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLRandomForestClassifier.ModelParameters) throws

Creates a Random Forest Classifier from the feature columns in the training data to predict the categories in the target column.

Deprecated

struct ModelParameters

Parameters that affect the process of training a model.

let modelParameters: MLRandomForestClassifier.ModelParameters

The underlying parameters used when training the model.

var featureColumns: [String]

The names of the columns you selected at initialization to train the classifier.

