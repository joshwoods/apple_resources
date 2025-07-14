

- Create ML
- MLStyleTransfer
-  MLStyleTransfer.ModelParameters 

Structure

# MLStyleTransfer.ModelParameters

Parameters that affect the training process of a style transfer model.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
struct ModelParameters
```

## Topics

### Creating parameters

init(algorithm: MLStyleTransfer.ModelParameters.ModelAlgorithmType, validation: MLStyleTransfer.ModelParameters.ValidationData, maxIterations: Int, textelDensity: Int, styleStrength: Int)

Creates a new set of training parameters for a style transfer model.

### Setting style transfer parameters

var algorithm: MLStyleTransfer.ModelParameters.ModelAlgorithmType

The style transfer task’s training algorithm that prioritizes either speed or quality.

var debugDescription: String

A text representation of the style transfer model parameters that’s suitable for output during debugging.

var description: String

A text representation of the style transfer model parameters.

var maxIterations: Int

The largest number of iterations the style transfer model can use during training.

var playgroundDescription: Any

A description of the style transfer model parameters shown in a playground.

var styleStrength: Int

The amount of influence the input style image has in the stylized image output.

var textelDensity: Int

The amount of detail the task applies from the input style image to the stylized image output.

var validation: MLStyleTransfer.ModelParameters.ValidationData

The style transfer model’s validation dataset.

### Describing parameters

enum ModelAlgorithmType

The style transfer training algorithm options.

enum ValidationData

The source of a validation dataset for a style transfer model.

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

### Supporting types

enum DataSource

A data source for a style transfer model.

