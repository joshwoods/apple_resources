

- Create ML
- MLObjectDetector
- MLObjectDetector.ModelParameters
-  algorithm 

Instance Property

# algorithm

The algorithm the training session uses to train the object detector.

macOS 11.0+

``` source
var algorithm: MLObjectDetector.ModelParameters.ModelAlgorithmType { get set }
```

## See Also

### Accessing the training parameters

var validation: MLObjectDetector.ModelParameters.ValidationData

The object detector’s validation dataset for the training session.

var batchSize: Int?

The number of images the training session can use in a training iteration.

var maxIterations: Int?

The maximum number of iterations the training session can use.

var gridSize: CGSize

The number of rectangles, vertically and horizontally, the training algorithm uses to analyze each input image.

