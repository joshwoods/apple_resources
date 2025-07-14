

- Vision
- VNPixelBufferObservation
-  featureName 

Instance Property

# featureName

A feature name that the CoreML model defines.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var featureName: String? { get }
```

## Discussion

This value is nil if the observation isn’t the result of a VNCoreMLRequest operation.

## See Also

### Parsing Observation Content

var pixelBuffer: CVPixelBuffer

The image that results from a request with image output.

