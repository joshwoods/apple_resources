

- Create ML
- MLHandPoseClassifier
-  MLHandPoseClassifier.ModelParameters 

Structure

# MLHandPoseClassifier.ModelParameters

A set of parameters that affect the training process of a hand pose classifier task.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
struct ModelParameters
```

## Topics

### Creating hand pose model parameters

init(validation: MLHandPoseClassifier.ModelParameters.ValidationData, batchSize: Int, maximumIterations: Int, augmentationOptions: MLHandPoseClassifier.ImageAugmentationOptions, algorithm: MLHandPoseClassifier.ModelParameters.ModelAlgorithmType)

Creates a set of training session parameters for a hand pose classifier task.

### Accessing hand pose training parameters

var maximumIterations: Int

The largest number of training iterations you allow the training session to use.

var batchSize: Int

The number of images the model training session uses for each training iteration.

var algorithm: MLHandPoseClassifier.ModelParameters.ModelAlgorithmType

The algorithm the training session uses to create the hand pose classifier.

var augmentationOptions: MLHandPoseClassifier.ImageAugmentationOptions

The variations the training session uses to add more variety to its training dataset.

var validation: MLHandPoseClassifier.ModelParameters.ValidationData

A dataset the hand pose classifier task uses to evaluate the model that’s distinct from the training dataset.

### Describing hand pose model parameters

var description: String

A text representation of the hand pose parameters.

var debugDescription: String

A text representation of the hand pose parameters suitable for debugging.

var playgroundDescription: Any

A description of the hand pose parameters that’s viewable in a playground.

### Parameter supporting types

struct ImageAugmentationOptions

Options a hand pose classification training session can use to generate additional training data from the images you provide.

enum ValidationData

A dataset a hand pose classifier task uses to validate the model during a training session.

enum ModelAlgorithmType

The hand pose classifier training algorithm options.

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

A hand pose classifier dataset that contains annotated images or hand joint location data.

