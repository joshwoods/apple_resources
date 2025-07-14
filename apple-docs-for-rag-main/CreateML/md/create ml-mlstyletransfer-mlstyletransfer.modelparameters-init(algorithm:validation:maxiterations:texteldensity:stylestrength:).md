

- Create ML
- MLStyleTransfer
- MLStyleTransfer.ModelParameters
-  init(algorithm:validation:maxIterations:textelDensity:styleStrength:) 

Initializer

# init(algorithm:validation:maxIterations:textelDensity:styleStrength:)

Creates a new set of training parameters for a style transfer model.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
init(
    algorithm: MLStyleTransfer.ModelParameters.ModelAlgorithmType = .cnn,
    validation: MLStyleTransfer.ModelParameters.ValidationData = .none,
    maxIterations: Int = MLStyleTransfer.__Defaults.maxIterations,
    textelDensity: Int = MLStyleTransfer.__Defaults.textelDensity,
    styleStrength: Int = MLStyleTransfer.__Defaults.styleStrength
)
```

## Discussion

- algorithm: The style transfer task’s training algorithm that prioritizes either speed or quality.

  - validation: The style transfer model’s validation dataset.

- maxIterations: The largest number of training iterations the style transfer model can use.

- textelDensity: The amount of detail the task applies from the input style image to the stylized image output.

- styleStrength: The amount of influence the style image has in the stylized image output.

