

- Create ML
- MLObjectDetector
-  makeTrainingSession(trainingData:annotationType:parameters:sessionParameters:) 

Type Method

# makeTrainingSession(trainingData:annotationType:parameters:sessionParameters:)

Creates an asynchronous object-detector training session.

macOS 11.0+

``` source
static func makeTrainingSession(
    trainingData: MLObjectDetector.DataSource,
    annotationType: MLObjectDetector.AnnotationType,
    parameters: MLObjectDetector.ModelParameters = ModelParameters(),
    sessionParameters: MLTrainingSessionParameters = __Defaults.sessionParameters
) throws -> MLTrainingSession
```

## Return Value

An MLTrainingSession that represents the object-detector training session.

## Discussion

Use resume(_:) to start the MLTrainingSession instance you get from this method.

- trainingData: The annotated images the task uses to train the object detector.

- annotationType: The format type of the image annotations in the data source.

- sessionParameters: An MLTrainingSessionParameters instance you use to configure the training session.

## See Also

### Training an object detector asynchronously

static func train(trainingData: MLObjectDetector.DataSource, annotationType: MLObjectDetector.AnnotationType, parameters: MLObjectDetector.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLObjectDetector>

Begins an asynchronous object-detector training session.

static func resume(MLTrainingSession&lt;MLObjectDetector>) throws -> MLJob&lt;MLObjectDetector>

Begins or continues an asynchronous object-detector training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLObjectDetector>

Creates an asynchronous training session for an object detector by restoring an existing training session’s state from its parameters.

