

- Vision
- VNPixelBufferObservation
-  pixelBuffer 

Instance Property

# pixelBuffer

The image that results from a request with image output.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var pixelBuffer: CVPixelBuffer { get }
```

## Discussion

VNCoreMLRequest produces observations that contain images in pixel buffer format. The confidence level is always `1.0`.

## See Also

### Parsing Observation Content

var featureName: String?

A feature name that the CoreML model defines.

