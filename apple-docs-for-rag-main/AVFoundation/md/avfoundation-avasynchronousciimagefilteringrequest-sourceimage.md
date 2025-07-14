

- AVFoundation
- AVAsynchronousCIImageFilteringRequest
-  sourceImage 

Instance Property

# sourceImage

The current video frame image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var sourceImage: CIImage { get }
```

## Discussion

To apply a Core Image filter to this image, assign it to the `inputImage` parameter of a CIFilter object, or use a CIImage convenience method such as the applyingFilter(_:parameters:) method.

The pixel format for this image is the BGRA8 format (of the kCVPixelFormatType_32BGRA type). Unlike when processing video with the AVAsynchronousVideoCompositionRequest class, the renderContext object’s renderTransform property is already applied to this image.

