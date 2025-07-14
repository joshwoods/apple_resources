

- AVFoundation
- AVCapturePhoto
-  isConstantColorFallbackPhoto 

Instance Property

# isConstantColorFallbackPhoto

A Boolean value that Indicates whether this photo is a fallback photo for a constant color capture.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
var isConstantColorFallbackPhoto: Bool { get }
```

## See Also

### Enabling Constant Color

var constantColorCenterWeightedMeanConfidenceLevel: Float

A score that summarizes the overall confidence level of a constant color photo.

var constantColorConfidenceMap: CVPixelBuffer?

A pixel buffer where each pixel value indicates how fully the system achieves the constant color effect in the corresponding region of the photo.

