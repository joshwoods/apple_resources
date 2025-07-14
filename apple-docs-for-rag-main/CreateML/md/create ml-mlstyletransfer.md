

- Create ML
-  MLStyleTransfer 

Structure

# MLStyleTransfer

A model you train to apply an image’s style to other images or videos.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
struct MLStyleTransfer
```

## Topics

### Training a style transfer model asynchronously

static func train(trainingData: MLStyleTransfer.DataSource, parameters: MLStyleTransfer.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLStyleTransfer>

Begins an asynchronous style transfer model-training session.

static func makeTrainingSession(trainingData: MLStyleTransfer.DataSource, parameters: MLStyleTransfer.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLStyleTransfer>

Creates an asynchronous training session for a style transfer model.

static func resume(MLTrainingSession&lt;MLStyleTransfer>) throws -> MLJob&lt;MLStyleTransfer>

Begins or continues an asynchronous style transfer model-training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLStyleTransfer>

Creates an asynchronous training session for a style transfer model by restoring an existing training session’s state from its parameters.

### Creating a style transfer model from a checkpoint

init(checkpoint: MLCheckpoint) throws

Creates a style transfer model from a training session checkpoint.

### Training a style transfer model synchronously

init(trainingData: MLStyleTransfer.DataSource, parameters: MLStyleTransfer.ModelParameters) throws

Creates a style transfer model with a training dataset represented by a data source.

### Stylizing an image

func stylize(image: CGImage) throws -> CGImage?

Applies the style the model learned to an image.

### Saving a style transfer model

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the style transfer model as a Core ML model file to a location in the file system.

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports the style transfer model as a Core ML model file to the file path.

### Downloading model assets

static func downloadAssets() throws

Initiates a download of the mlmodel assets required for Style Transfer training. This will be performed automatically if needed at training time, but can be run independently prior to training.

### Describing a style transfer model

var description: String

A text representation of the style transfer model.

var debugDescription: String

A text representation of the style transfer model that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the style transfer model shown in a playground.

### Supporting types

enum DataSource

A data source for a style transfer model.

struct ModelParameters

Parameters that affect the training process of a style transfer model.

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

struct MLActionClassifier

A model you train with videos to classify a person’s body movements.

struct MLHandActionClassifier

A task that creates a hand action classification model by training with videos of people’s hand movements that you provide.

