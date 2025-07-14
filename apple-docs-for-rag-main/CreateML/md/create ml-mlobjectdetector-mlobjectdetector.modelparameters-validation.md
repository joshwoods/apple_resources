

- Create ML
- MLObjectDetector
- MLObjectDetector.ModelParameters
-  validation 

Instance Property

# validation

The object detector’s validation dataset for the training session.

macOS 10.15+

``` source
var validation: MLObjectDetector.ModelParameters.ValidationData
```

## See Also

### Accessing the training parameters

var batchSize: Int?

The number of images the training session can use in a training iteration.

var maxIterations: Int?

The maximum number of iterations the training session can use.

var algorithm: MLObjectDetector.ModelParameters.ModelAlgorithmType

The algorithm the training session uses to train the object detector.

var gridSize: CGSize

The number of rectangles, vertically and horizontally, the training algorithm uses to analyze each input image.

