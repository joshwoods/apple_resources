

- Create ML
- MLStyleTransfer
- MLStyleTransfer.ModelParameters
-  playgroundDescription 

Instance Property

# playgroundDescription

A description of the style transfer model parameters shown in a playground.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
var playgroundDescription: Any { get }
```

## See Also

### Setting style transfer parameters

var algorithm: MLStyleTransfer.ModelParameters.ModelAlgorithmType

The style transfer task’s training algorithm that prioritizes either speed or quality.

var debugDescription: String

A text representation of the style transfer model parameters that’s suitable for output during debugging.

var description: String

A text representation of the style transfer model parameters.

var maxIterations: Int

The largest number of iterations the style transfer model can use during training.

var styleStrength: Int

The amount of influence the input style image has in the stylized image output.

var textelDensity: Int

The amount of detail the task applies from the input style image to the stylized image output.

var validation: MLStyleTransfer.ModelParameters.ValidationData

The style transfer model’s validation dataset.

