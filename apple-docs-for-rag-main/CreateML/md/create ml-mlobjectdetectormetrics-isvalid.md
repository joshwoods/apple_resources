

- Create ML
- MLObjectDetectorMetrics
-  isValid 

Instance Property

# isValid

A Boolean value indicating whether the object detector model was able to calculate metrics.

macOS 10.15+

``` source
var isValid: Bool { get }
```

## Discussion

Your metrics may be invalid if you attempt to perform evaluation on images with annotations that don’t match the annotations of your training examples.

## See Also

### Handling errors

var error: (any Error)?

The underlying error present when the metrics are invalid.

