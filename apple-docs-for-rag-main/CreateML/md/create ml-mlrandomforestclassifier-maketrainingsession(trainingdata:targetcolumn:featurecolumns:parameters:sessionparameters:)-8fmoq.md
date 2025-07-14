

- Create ML
- MLRandomForestClassifier
-  makeTrainingSession(trainingData:targetColumn:featureColumns:parameters:sessionParameters:) 

Type Method

# makeTrainingSession(trainingData:targetColumn:featureColumns:parameters:sessionParameters:)

Creates or restores a training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
static func makeTrainingSession(
    trainingData: DataFrame,
    targetColumn: String,
    featureColumns: [String]? = nil,
    parameters: MLRandomForestClassifier.ModelParameters = .init(),
    sessionParameters: MLTrainingSessionParameters = _defaultSessionParameters
) throws -> MLTrainingSession
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

A `MLTrainingSession` that can be used to start or resume training.

## See Also

### Creating a training session

static func makeTrainingSession(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLRandomForestClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLRandomForestClassifier>

Creates or restores a training session.

