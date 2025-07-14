

- Create ML
- MLObjectDetector
-  restoreTrainingSession(sessionParameters:) 

Type Method

# restoreTrainingSession(sessionParameters:)

Creates an asynchronous training session for an object detector by restoring an existing training session’s state from its parameters.

macOS 11.0+

``` source
static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession
```

## Return Value

An MLTrainingSession that represents the object-detector training session.

## Discussion

Use resume(_:) to start the MLTrainingSession instance you get from this method.

- sessionParameters: The MLTrainingSessionParameters instance you used to create the training session with makeTrainingSession(trainingData:annotationType:parameters:sessionParameters:).

## See Also

### Training an object detector asynchronously

static func train(trainingData: MLObjectDetector.DataSource, annotationType: MLObjectDetector.AnnotationType, parameters: MLObjectDetector.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLObjectDetector>

Begins an asynchronous object-detector training session.

static func makeTrainingSession(trainingData: MLObjectDetector.DataSource, annotationType: MLObjectDetector.AnnotationType, parameters: MLObjectDetector.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLObjectDetector>

Creates an asynchronous object-detector training session.

static func resume(MLTrainingSession&lt;MLObjectDetector>) throws -> MLJob&lt;MLObjectDetector>

Begins or continues an asynchronous object-detector training session.

