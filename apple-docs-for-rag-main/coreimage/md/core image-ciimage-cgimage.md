

- Core Image
- CIImage
-  cgImage 

Instance Property

# cgImage

The CoreGraphics image object this image was created from, if applicable.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var cgImage: CGImage? { get }
```

## Discussion

If this image was created using the init(cgImage:) or init(contentsOf:) initializer, this property’s value is the CGImage object that provides the image’s underlying image data. Otherwise, this property’s value is `nil`—in this case you can obtain a CoreGraphics image by rendering the image with the CIContext createCGImage(_:from:) method.

## See Also

### Accessing Original Image Content

var pixelBuffer: CVPixelBuffer?

The CoreVideo pixel buffer this image was created from, if applicable.

var depthData: AVDepthData?

AVDepthData representation of the depth image.

var portraitEffectsMatte: AVPortraitEffectsMatte?

AVPortraitEffectsMatte representation of portrait effects.

var semanticSegmentationMatte: AVSemanticSegmentationMatte?

