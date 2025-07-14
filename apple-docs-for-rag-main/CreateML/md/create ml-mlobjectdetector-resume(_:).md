

- Create ML
- MLObjectDetector
-  resume(\_:) 

Type Method

# resume(\_:)

Begins or continues an asynchronous object-detector training session.

macOS 11.0+

``` source
static func resume(_ session: MLTrainingSession) throws -> MLJob
```

## Return Value

An MLJob that represents the object-detector training session.

## Discussion

Use this method to start or resume a training session you get from makeTrainingSession(trainingData:annotationType:parameters:sessionParameters:) or restoreTrainingSession(sessionParameters:).

- session: An MLTrainingSession instance that represents the training session.

## See Also

### Training an object detector asynchronously

static func train(trainingData: MLObjectDetector.DataSource, annotationType: MLObjectDetector.AnnotationType, parameters: MLObjectDetector.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLObjectDetector>

Begins an asynchronous object-detector training session.

static func makeTrainingSession(trainingData: MLObjectDetector.DataSource, annotationType: MLObjectDetector.AnnotationType, parameters: MLObjectDetector.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLObjectDetector>

Creates an asynchronous object-detector training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLObjectDetector>

Creates an asynchronous training session for an object detector by restoring an existing training session’s state from its parameters.

