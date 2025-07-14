

- Create ML
- MLStyleTransfer
- MLStyleTransfer.ModelParameters
-  algorithm 

Instance Property

# algorithm

The style transfer task’s training algorithm that prioritizes either speed or quality.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
var algorithm: MLStyleTransfer.ModelParameters.ModelAlgorithmType
```

## Discussion

You choose the task’s training algorithm based on your intended use for this model.

Use MLStyleTransfer.ModelParameters.ModelAlgorithmType.cnnLite to train a model that prioritizes speed to stylize images with low latency, typically for frames of a video stream. Otherwise, select MLStyleTransfer.ModelParameters.ModelAlgorithmType.cnn to train a model that applies a higher-quality stylization, typically for a still image.

## See Also

### Setting style transfer parameters

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

