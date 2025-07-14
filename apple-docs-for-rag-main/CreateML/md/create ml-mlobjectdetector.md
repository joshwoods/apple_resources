

- Create ML
-  MLObjectDetector 

Structure

# MLObjectDetector

A model you train to classify one or more objects within an image.

macOS 10.15+

``` source
struct MLObjectDetector
```

## Mentioned in 

Building an object detector data source

## Overview

Use an MLObjectDetector task to train a machine learning model that can identify items, or *objects*, within an image. For example, you can train an object detector to recognize breakfast items on a table, such as bananas, croissants, and beverages.

You create an object detector training it with a combination of images and annotations for each object within an image. Then save it as a Core ML model and use it in your app to recognize similar items.

## Topics

### Creating a data source

Building an object detector data source

Arrange your training data for an object detector in one of several different structured ways.

### Training an object detector asynchronously

static func train(trainingData: MLObjectDetector.DataSource, annotationType: MLObjectDetector.AnnotationType, parameters: MLObjectDetector.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLObjectDetector>

Begins an asynchronous object-detector training session.

static func makeTrainingSession(trainingData: MLObjectDetector.DataSource, annotationType: MLObjectDetector.AnnotationType, parameters: MLObjectDetector.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLObjectDetector>

Creates an asynchronous object-detector training session.

static func resume(MLTrainingSession&lt;MLObjectDetector>) throws -> MLJob&lt;MLObjectDetector>

Begins or continues an asynchronous object-detector training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLObjectDetector>

Creates an asynchronous training session for an object detector by restoring an existing training session’s state from its parameters.

### Creating an object detector from a checkpoint

init(checkpoint: MLCheckpoint) throws

Creates an object detector from a training session checkpoint.

### Training an object detector synchronously

init(trainingData: MLObjectDetector.DataSource, parameters: MLObjectDetector.ModelParameters, annotationType: MLObjectDetector.AnnotationType) throws

Creates an object detector with a data source.

init(trainingData: MLDataTable, imageColumn: String, annotationColumn: String, annotationType: MLObjectDetector.AnnotationType, parameters: MLObjectDetector.ModelParameters) throws

Creates an object detector with a data table.

Deprecated

### Assessing model accuracy

var trainingMetrics: MLObjectDetectorMetrics

Measurements of the object detector’s performance on the training dataset.

var validationMetrics: MLObjectDetectorMetrics

Measurements of the object detector’s performance on the validation dataset.

### Evaluating an object detector

func evaluation(on: MLObjectDetector.DataSource) -> MLObjectDetectorMetrics

Generates metrics by evaluating the object detector’s performance using annotated images in a data source.

func evaluation(on: MLDataTable, imageColumn: String, annotationColumn: String) -> MLObjectDetectorMetrics

Generates metrics by evaluating the object detector’s performance using annotated images in a data table.

Deprecated

### Testing an object detector

func prediction(from: URL) throws -> MLObjectDetector.DetectedObjects

Locates objects in an image and generates an annotation for each object it detects.

func predictions(from: [URL]) throws -> [MLObjectDetector.DetectedObjects]

Locates objects in an array of images and generates an array of annotation collections, one for each input image.

typealias DetectedObjects

An array of annotations that represent the items an object detector found in an image.

struct ObjectAnnotation

The label, location, and confidence score of an item the object detector found in an image.

### Saving an object detector

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the object detector as a Core ML model file.

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports the object detector as a Core ML model file.

### Inspecting an object detector model

var model: MLModel

The object detector’s underlying Core ML model instance.

let modelParameters: MLObjectDetector.ModelParameters

The model configuration parameters the object detector used during its training session.

### Describing an object detector

var description: String

A text representation of the object detector.

var debugDescription: String

A text representation of the object detector that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the object detector within a playground.

### Supporting types

enum DataSource

A data source for an object detector.

enum AnnotationType

The available types of image annotations.

struct ModelParameters

Parameters that affect the process of training an object detection model.

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

struct MLImageClassifier

A model you train to classify images.

struct MLHandPoseClassifier

A task that creates a hand pose classification model by training with images of people’s hands that you provide.

