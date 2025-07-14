

- Core Image
- CIImage
-  pixelBuffer 

Instance Property

# pixelBuffer

The CoreVideo pixel buffer this image was created from, if applicable.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var pixelBuffer: CVPixelBuffer? { get }
```

## Discussion

If this image was create using the init(cvPixelBuffer:) initializer, this property’s value is the CVPixelBuffer object that provides the image’s underlying image data. Do not modify the contents of this pixel buffer; doing so will cause undefined rendering results.

Otherwise, this property’s value is `nil`—in this case you can obtain a pixel buffer by rendering the image with the CIContext render(_:to:) method.

## See Also

### Accessing Original Image Content

var cgImage: CGImage?

The CoreGraphics image object this image was created from, if applicable.

var depthData: AVDepthData?

AVDepthData representation of the depth image.

var portraitEffectsMatte: AVPortraitEffectsMatte?

AVPortraitEffectsMatte representation of portrait effects.

var semanticSegmentationMatte: AVSemanticSegmentationMatte?

