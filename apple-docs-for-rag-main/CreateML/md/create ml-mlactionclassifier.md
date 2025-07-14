

- Create ML
-  MLActionClassifier 

Structure

# MLActionClassifier

A model you train with videos to classify a person’s body movements.

macOS 11.0+

``` source
struct MLActionClassifier
```

## Topics

### Training an action classifier asynchronously

static func train(trainingData: MLActionClassifier.DataSource, parameters: MLActionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLActionClassifier>

Begins an asynchronous action classifier training session.

static func makeTrainingSession(trainingData: MLActionClassifier.DataSource, parameters: MLActionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLActionClassifier>

Creates an asynchronous training session for an action classifier.

static func resume(MLTrainingSession&lt;MLActionClassifier>) throws -> MLJob&lt;MLActionClassifier>

Begins or continues an asynchronous action classifier training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLActionClassifier>

Creates an asynchronous training session for an action classifier by restoring an existing training session’s state from its parameters.

### Creating an action classifier from a checkpoint

init(checkpoint: MLCheckpoint) throws

Creates an action classifier from a training session checkpoint.

### Training an action classifier synchronously

init(trainingData: MLActionClassifier.DataSource, parameters: MLActionClassifier.ModelParameters) throws

Creates an action classifier with a training dataset represented by a data source.

### Evaluating an action classifier

var trainingMetrics: MLClassifierMetrics

Measurements of the action classifier’s performance on the training dataset.

var validationMetrics: MLClassifierMetrics

Measurements of the action classifier’s performance on the validation dataset.

func evaluation(on: MLActionClassifier.DataSource) throws -> MLClassifierMetrics

Generates metrics describing the action classifier’s performance on labeled videos represented by a data source.

### Testing an action classifier

func prediction(from: URL) throws -> [MLActionClassifier.Prediction]

Generates a prediction for each action the classifier recognizes in the video.

func predictions(from: [URL]) throws -> [[MLActionClassifier.Prediction]]

Generates a sequence of predictions for each video input.

struct Prediction

A collection of predictions, each paired with its confidence, for a range of video frames.

### Saving an action classifier

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the action classifier as a Core ML model file to a location in the file system.

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports the action classifier as a Core ML model file to the file path.

### Inspecting an action classifier model

var model: MLModel

The underlying Core ML model of the action classifier stored in memory.

let modelParameters: MLActionClassifier.ModelParameters

The model configuration parameters the action classifier used during its training session.

### Describing an action classifier

var description: String

A text representation of the action classifier.

var debugDescription: String

A text representation of the action classifier that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the action classifier shown in a playground.

### Supporting types

enum DataSource

A data source for an action classifier.

struct ModelParameters

Parameters that affect the training process of an action classifier.

### Structures

struct VideoAugmentationOptions

The video augmentations for an action classifier training session.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomPlaygroundDisplayConvertible Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomPlaygroundDisplayConvertible
- CustomStringConvertible
- Sendable

## See Also

### Video Models

Creating an Action Classifier Model

Train a machine learning model to recognize a person’s body movements.

Detecting Human Actions in a Live Video Feed

Identify body movements by sending a person’s pose data from a series of video frames to an action-classification model.

struct MLHandActionClassifier

A task that creates a hand action classification model by training with videos of people’s hand movements that you provide.

struct MLStyleTransfer

A model you train to apply an image’s style to other images or videos.

