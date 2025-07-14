

- Create ML
-  MLHandActionClassifier 

Structure

# MLHandActionClassifier

A task that creates a hand action classification model by training with videos of people’s hand movements that you provide.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
struct MLHandActionClassifier
```

## Topics

### Training a hand action classifier asynchronously

static func train(trainingData: MLHandActionClassifier.DataSource, parameters: MLHandActionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLHandActionClassifier>

Begins an asynchronous hand action classifier’s training session.

static func makeTrainingSession(trainingData: MLHandActionClassifier.DataSource, parameters: MLHandActionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLHandActionClassifier>

Creates an asynchronous hand action classifier’s training session.

static func resume(MLTrainingSession&lt;MLHandActionClassifier>) throws -> MLJob&lt;MLHandActionClassifier>

Begins or continues an asynchronous hand action classifier’s training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLHandActionClassifier>

Recreates an asynchronous hand action classifier’s training session by restoring its saved state from the file system.

### Creating a hand action classifier from a checkpoint

init(checkpoint: MLCheckpoint) throws

Creates a hand action classifier from a training session checkpoint.

### Training a hand action classifier synchronously

init(trainingData: MLHandActionClassifier.DataSource, parameters: MLHandActionClassifier.ModelParameters) throws

Creates a hand action classifier by starting a synchronous training session.

### Evaluating a hand action classifier

var trainingMetrics: MLClassifierMetrics

Measurements of the hand action classifier’s performance on the training dataset.

var validationMetrics: MLClassifierMetrics

Measurements of the hand action classifier’s performance on the validation dataset.

func evaluation(on: MLHandActionClassifier.DataSource) throws -> MLClassifierMetrics

Generates metrics describing the hand action classifier’s performance on labeled videos.

### Testing a hand action classifier

func prediction(from: URL) throws -> [MLHandActionClassifier.Prediction]

Generates a hand action prediction for a video.

func predictions(from: [URL]) throws -> [[MLHandActionClassifier.Prediction]]

Generates an array of hand action predictions for each video in a URL array.

struct Prediction

A collection of predictions, each paired with its confidence, for a range of video frames.

### Saving a hand action classifier

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the hand action classifier as a CoreML model file.

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports the hand action classifier as a Core ML model file.

### Inspecting a hand action classifier model

var model: MLModel

The underlying Core ML model of the hand action classifier stored in memory.

let modelParameters: MLHandActionClassifier.ModelParameters

The hand action model’s configuration parameters.

### Describing a hand action classifier

var description: String

A text representation of the hand action classifier.

var debugDescription: String

A text representation of the hand action classifier suitable for debugging.

var playgroundDescription: Any

A description of the hand action classifier that’s viewable in a playground.

### Supporting types

enum DataSource

A hand action classifier dataset that contains annotated videos or hand joint location data.

struct ModelParameters

A set of parameters that affect the training process of a hand action classifier task.

### Structures

struct VideoAugmentationOptions

Options a hand action classification training session can use to generate additional training data from the videos you provide.

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

## See Also

### Video Models

Creating an Action Classifier Model

Train a machine learning model to recognize a person’s body movements.

Detecting Human Actions in a Live Video Feed

Identify body movements by sending a person’s pose data from a series of video frames to an action-classification model.

struct MLActionClassifier

A model you train with videos to classify a person’s body movements.

struct MLStyleTransfer

A model you train to apply an image’s style to other images or videos.

