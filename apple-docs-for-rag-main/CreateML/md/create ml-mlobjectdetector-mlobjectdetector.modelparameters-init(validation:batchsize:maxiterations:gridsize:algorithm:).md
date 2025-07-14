

- Create ML
- MLObjectDetector
- MLObjectDetector.ModelParameters
-  init(validation:batchSize:maxIterations:gridSize:algorithm:) 

Initializer

# init(validation:batchSize:maxIterations:gridSize:algorithm:)

Creates a model parameters instance for an object-detector training session.

macOS 11.0+

``` source
init(
    validation: MLObjectDetector.ModelParameters.ValidationData = .split(strategy: .automatic),
    batchSize: Int? = nil,
    maxIterations: Int? = nil,
    gridSize: CGSize = CGSize(width: 13, height: 13),
    algorithm: MLObjectDetector.ModelParameters.ModelAlgorithmType = .darknetYolo
)
```

## Discussion

- validation: An MLObjectDetector.ModelParameters.ValidationData instance that contains your validation dataset.

- batchSize: The number of images the object detector uses for each training iteration. If you don’t have a preference, set this parameter to `nil` to tell Create ML to use an appropriate value when it trains the model.

- maxIterations: The largest number of training iterations the object detector can use. If you don’t have a preference, set this parameter to `nil` to tell Create ML to use an appropriate value when it trains the model.

- gridSize: The number of rectangles, vertically and horizontally, the training algorithm uses to analyze each input image.

- algorithm: The algorithm the training session uses to train the object detector.

## See Also

### Creating object detector parameters

init(validation: MLObjectDetector.ModelParameters.ValidationData, batchSize: Int?, maxIterations: Int?)

Creates a model parameters instance for an object-detector training session set to use the full network algorithm.

init(validationData: MLObjectDetector.DataSource, batchSize: Int?, maxIterations: Int?) throws

Creates a model parameters instance for an object-detector training session set to use the full network algorithm.

Deprecated

