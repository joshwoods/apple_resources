

- Create ML
- MLRandomForestClassifier
-  train(trainingData:targetColumn:featureColumns:parameters:sessionParameters:) 

Type Method

# train(trainingData:targetColumn:featureColumns:parameters:sessionParameters:)

Trains a random forest classifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
static func train(
    trainingData: DataFrame,
    targetColumn: String,
    featureColumns: [String]? = nil,
    parameters: MLRandomForestClassifier.ModelParameters = ModelParameters(),
    sessionParameters: MLTrainingSessionParameters = _defaultSessionParameters
) throws -> MLJob
```

## Parameters 

`trainingData`  

A `DataFrame` specifying training data.

`targetColumn`  

A String specifying the target column name in the trainingData

`featureColumns`  

An optional list of Strings specifying feature columns to be used to predict the target, if not provided, default to use all the other columns in the trainingData, except the one specified by targetColumn

`parameters`  

Model training parameters. See `MLRandomForestClassifier.ModelParameters` for the defaults.

`sessionParameters`  

Training session parameters. See `MLTrainingSessionParameters` for the defaults.

## Return Value

A `MLJob` that can be used to observe training progress.

## Discussion

If `sessionDirectory` is provided it will save training progress. If there is progress already saved training will resume from the last checkpoint.

## See Also

### Training a random forest classifier

static func train(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLRandomForestClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLRandomForestClassifier>

Trains a random forest classifier.

