

- Create ML
- MLObjectDetector
-  MLObjectDetector.ModelParameters 

Structure

# MLObjectDetector.ModelParameters

Parameters that affect the process of training an object detection model.

macOS 10.15+

``` source
struct ModelParameters
```

## Overview

Customize the training process of an object detector by creating an MLObjectDetector.ModelParameters instance and passing it to an object detector’s initializer. You can explicitly set values for maxIterations and batchSize. You can also explicitly define the validation dataset to override the default behavior, which uses a random selection of your training dataset for validation.

## Topics

### Creating object detector parameters

init(validation: MLObjectDetector.ModelParameters.ValidationData, batchSize: Int?, maxIterations: Int?)

Creates a model parameters instance for an object-detector training session set to use the full network algorithm.

init(validation: MLObjectDetector.ModelParameters.ValidationData, batchSize: Int?, maxIterations: Int?, gridSize: CGSize, algorithm: MLObjectDetector.ModelParameters.ModelAlgorithmType)

Creates a model parameters instance for an object-detector training session.

init(validationData: MLObjectDetector.DataSource, batchSize: Int?, maxIterations: Int?) throws

Creates a model parameters instance for an object-detector training session set to use the full network algorithm.

Deprecated

### Accessing the training parameters

var validation: MLObjectDetector.ModelParameters.ValidationData

The object detector’s validation dataset for the training session.

var batchSize: Int?

The number of images the training session can use in a training iteration.

var maxIterations: Int?

The maximum number of iterations the training session can use.

var algorithm: MLObjectDetector.ModelParameters.ModelAlgorithmType

The algorithm the training session uses to train the object detector.

var gridSize: CGSize

The number of rectangles, vertically and horizontally, the training algorithm uses to analyze each input image.

### Describing the model parameters

var description: String

A text representation of the model parameters.

var debugDescription: String

A text representation of the model parameters that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the model parameters within a playground.

### Supporting types

enum ValidationData

A validation dataset for an object detector.

enum ModelAlgorithmType

An object-detector training algorithm.

### Enumerations

enum FeatureExtractorType

The underlying base model that extracts image features for an object-detector training session.

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

### Supporting types

enum DataSource

A data source for an object detector.

enum AnnotationType

The available types of image annotations.

