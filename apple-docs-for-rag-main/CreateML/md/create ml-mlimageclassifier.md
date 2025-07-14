

- Create ML
-  MLImageClassifier 

Structure

# MLImageClassifier

A model you train to classify images.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
struct MLImageClassifier
```

## Mentioned in 

Improving Your Model’s Accuracy

Creating an Image Classifier Model

## Overview

Use an image classifier to train a machine learning model that you can include in your app to categorize images.

When you create the model, you give it a training dataset made up of labeled images, along with parameters that control the training process. For example, you can provide the model with images of elephants and giraffes, in two folders labeled `Elephant` and `Giraffe`, to train it to recognize these animals.

After training completes, you evaluate the trained model by showing it a testing dataset containing labeled images that the model hasn’t seen before. The metrics that come from this evaluation tell you whether the model performs well enough. For example, you can see how often the elephant and giraffe classifier mistakes a giraffe for an elephant. When the model makes too many mistakes, you can add more or better training data, or change the parameters, and try again.

When your model does perform well enough, you save it as a Core ML model file with the `mlmodel` extension. You can then import this model file into an app—like the Classifying Images with Vision and Core ML sample code project—that uses a Core ML model file to classify images.

## Topics

### Training an image classifier asynchronously

static func makeTrainingSession(trainingData: MLImageClassifier.DataSource, parameters: MLImageClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLImageClassifier>

Creates or restores a training session.

static func train(trainingData: MLImageClassifier.DataSource, parameters: MLImageClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLImageClassifier>

Begins an asynchronous image classifier training session with a training dataset represented by a data source.

static func resume(MLTrainingSession&lt;MLImageClassifier>) throws -> MLJob&lt;MLImageClassifier>

Begins or continues an asynchronous image classifier training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLImageClassifier>

Creates an asynchronous training session for an image classifier by restoring an existing training session’s state from its parameters.

### Creating an image classifier from a checkpoint

init(checkpoint: MLCheckpoint) throws

Creates an image classifier from a training session checkpoint.

### Training an image classifier synchronously

init(trainingData: MLImageClassifier.DataSource, parameters: MLImageClassifier.ModelParameters) throws

Creates an image classifier with a training dataset represented by a data source.

init(trainingData: [String : [URL]], parameters: MLImageClassifier.ModelParameters) throws

Creates an image classifier with a training dataset represented by a dictionary.

Deprecated

### Assessing model accuracy

var trainingMetrics: MLClassifierMetrics

Measurements of the classifier’s performance on the training data set.

var validationMetrics: MLClassifierMetrics

Measurements of the image classifier’s performance on the validation dataset.

### Evaluating an image classifier

func evaluation(on: MLImageClassifier.DataSource) -> MLClassifierMetrics

Generates metrics describing the image classifier’s performance on labeled images represented by a data source.

func evaluation(on: [String : [URL]]) -> MLClassifierMetrics

Generates metrics describing the image classifier’s performance on labeled images represented by a dictionary.

Deprecated

### Testing an image classifier

func prediction(from: CGImage) throws -> String

Generates a prediction for an image.

func prediction(from: URL) throws -> String

Generates a prediction for an image at the URL.

func predictions(from: [URL]) throws -> [String]

Generates predictions for an array of images.

### Saving an image classifier

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the image classifier as a Core ML model file to a location in the file system.

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports the image classifier as a Core ML model file to the file path.

### Inspecting an image classifier model

var model: MLModel

The underlying Core ML model of the image classifier stored in memory.

let modelParameters: MLImageClassifier.ModelParameters

The model configuration parameters the image classifier used during its training session.

### Describing an image classifier

var description: String

A text representation of the image classifier.

var debugDescription: String

A text representation of the image classifier that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the image classifier shown in a playground.

### Supporting types

enum DataSource

A data source for an image classifier.

struct ModelParameters

Parameters that affect the process of training an image classifier model.

### Structures

struct CustomFeatureExtractor

A custom feature extractor a training session uses to train an image classifier.

struct ImageAugmentationOptions

The variations that the training process can use to generate more training data from the training data you provide.

### Enumerations

enum FeatureExtractorType

The underlying base model that extracts image features for image classifier training session.

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

### Image Models

Creating an Image Classifier Model

Train a machine learning model to classify images, and add it to your Core ML app.

struct MLObjectDetector

A model you train to classify one or more objects within an image.

struct MLHandPoseClassifier

A task that creates a hand pose classification model by training with images of people’s hands that you provide.

