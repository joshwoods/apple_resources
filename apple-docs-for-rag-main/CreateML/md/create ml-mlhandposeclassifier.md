

- Create ML
-  MLHandPoseClassifier 

Structure

# MLHandPoseClassifier

A task that creates a hand pose classification model by training with images of people’s hands that you provide.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
struct MLHandPoseClassifier
```

## Topics

### Training a hand pose classifier asynchronously

static func train(trainingData: MLHandPoseClassifier.DataSource, parameters: MLHandPoseClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLHandPoseClassifier>

Begins an asynchronous hand pose classifier’s training session.

static func makeTrainingSession(trainingData: MLHandPoseClassifier.DataSource, parameters: MLHandPoseClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLHandPoseClassifier>

Creates an asynchronous hand pose classifier’s training session.

static func resume(MLTrainingSession&lt;MLHandPoseClassifier>) throws -> MLJob&lt;MLHandPoseClassifier>

Begins or continues an asynchronous hand pose classifier’s training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLHandPoseClassifier>

Recreates an asynchronous hand pose classifier’s training session by restoring its saved state from the file system.

### Creating a hand pose classifier from a checkpoint

init(checkpoint: MLCheckpoint) throws

Creates a hand pose classifier from a training session checkpoint.

### Training a hand pose classifier synchronously

init(trainingData: MLHandPoseClassifier.DataSource, parameters: MLHandPoseClassifier.ModelParameters) throws

Creates a hand pose classifier by starting a synchronous training session.

### Evaluating a hand pose classifier

var trainingMetrics: MLClassifierMetrics

Measurements of the hand pose classifier’s performance on the training dataset.

var validationMetrics: MLClassifierMetrics

Measurements of the hand pose classifier’s performance on the validation dataset.

func evaluation(on: MLHandPoseClassifier.DataSource) throws -> MLClassifierMetrics

Generates metrics that describe the hand pose classifier’s performance with a dataset of labeled images.

### Testing a hand pose classifier

func prediction(from: URL) throws -> [(label: String, confidence: Double)]

Generates a hand pose prediction for an image.

func predictions(from: [URL]) throws -> [[(label: String, confidence: Double)]]

Generates an array of hand pose predictions for each image in a URL array.

### Saving a hand pose classifier

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the hand pose classifier as a CoreML model file.

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports the hand pose classifier as a Core ML model file.

### Inspecting a hand pose classifier model

var model: MLModel

The underlying Core ML model of the hand pose classifier stored in memory.

let modelParameters: MLHandPoseClassifier.ModelParameters

The hand pose model’s configuration parameters.

### Describing a hand pose classifier

var description: String

A text representation of the hand pose classifier.

var debugDescription: String

A text representation of the hand pose classifier suitable for debugging.

var playgroundDescription: Any

A description of the hand pose classifier that’s viewable in a playground.

### Supporting types

enum DataSource

A hand pose classifier dataset that contains annotated images or hand joint location data.

struct ModelParameters

A set of parameters that affect the training process of a hand pose classifier task.

### Structures

struct ImageAugmentationOptions

Options a hand pose classification training session can use to generate additional training data from the images you provide.

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

### Image Models

Creating an Image Classifier Model

Train a machine learning model to classify images, and add it to your Core ML app.

struct MLImageClassifier

A model you train to classify images.

struct MLObjectDetector

A model you train to classify one or more objects within an image.

