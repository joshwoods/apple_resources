

- Create ML
- MLObjectDetector
- MLObjectDetector.ModelParameters
-  batchSize 

Instance Property

# batchSize

The number of images the training session can use in a training iteration.

macOS 10.15+

``` source
var batchSize: Int?
```

## Discussion

If you don’t have a preference, set this property to `nil` to tell Create ML to use an appropriate value when it trains the model.

## See Also

### Accessing the training parameters

var validation: MLObjectDetector.ModelParameters.ValidationData

The object detector’s validation dataset for the training session.

var maxIterations: Int?

The maximum number of iterations the training session can use.

var algorithm: MLObjectDetector.ModelParameters.ModelAlgorithmType

The algorithm the training session uses to train the object detector.

var gridSize: CGSize

The number of rectangles, vertically and horizontally, the training algorithm uses to analyze each input image.

