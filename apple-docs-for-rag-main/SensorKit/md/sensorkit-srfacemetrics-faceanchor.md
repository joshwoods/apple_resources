

- SensorKit
- SRFaceMetrics
-  faceAnchor 

Instance Property

# faceAnchor

The anchor for the face that the sensor detects in front of the camera.

iOS 17.0+iPadOS 17.0+

``` source
@NSCopying
var faceAnchor: ARFaceAnchor { get }
```

## See Also

### Getting face analytics

var partialFaceExpressions: [SRFaceMetricsExpression]

The partial face expressions that the algorithm detects.

var wholeFaceExpressions: [SRFaceMetricsExpression]

The whole face expressions that the algorithm detects.

class SRFaceMetricsExpression

An object that represents a facial expression.

