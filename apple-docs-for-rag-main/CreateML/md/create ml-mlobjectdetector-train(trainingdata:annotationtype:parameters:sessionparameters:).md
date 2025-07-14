

- Create ML
- MLObjectDetector
-  train(trainingData:annotationType:parameters:sessionParameters:) 

Type Method

# train(trainingData:annotationType:parameters:sessionParameters:)

Begins an asynchronous object-detector training session.

macOS 11.0+

``` source
static func train(
    trainingData: MLObjectDetector.DataSource,
    annotationType: MLObjectDetector.AnnotationType,
    parameters: MLObjectDetector.ModelParameters = ModelParameters(),
    sessionParameters: MLTrainingSessionParameters = __Defaults.sessionParameters
) throws -> MLJob
```

## Return Value

An MLJob that represents the object-detector training session.

## Discussion

- trainingData: The annotated images the task uses to train the object detector.

- annotationType: The format your data source uses for its image annotations.

- sessionParameters: An MLTrainingSessionParameters instance you use to configure the training session.

## See Also

### Training an object detector asynchronously

static func makeTrainingSession(trainingData: MLObjectDetector.DataSource, annotationType: MLObjectDetector.AnnotationType, parameters: MLObjectDetector.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLObjectDetector>

Creates an asynchronous object-detector training session.

static func resume(MLTrainingSession&lt;MLObjectDetector>) throws -> MLJob&lt;MLObjectDetector>

Begins or continues an asynchronous object-detector training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLObjectDetector>

Creates an asynchronous training session for an object detector by restoring an existing training session’s state from its parameters.

