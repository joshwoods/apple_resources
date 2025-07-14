

- Vision
- VNFaceLandmarkRegion2D
-  precisionEstimatesPerPoint 

Instance Property

# precisionEstimatesPerPoint

Requests an array of precision estimates for each landmark point.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
@nonobjc
var precisionEstimatesPerPoint: [Float]? { get }
```

## Discussion

This property is only populated when you configure your VNDetectFaceLandmarksRequest object with VNRequestFaceLandmarksConstellation.constellation76Points. For other constellation types, this array is set to `nil`.

## See Also

### Specifying Region Properties

var normalizedPoints: [CGPoint]

The array of normalized landmark points.

