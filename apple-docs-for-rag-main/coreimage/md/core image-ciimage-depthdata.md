

- Core Image
- CIImage
-  depthData 

Instance Property

# depthData

AVDepthData representation of the depth image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var depthData: AVDepthData? { get }
```

## Discussion

Returns an AVDepthData if the CIImage was created with imageWithData: or imageWithContentsOfURL: and one of the options auxiliaryDepth or auxiliaryDisparity, otherwise `nil`.

## See Also

### Accessing Original Image Content

var cgImage: CGImage?

The CoreGraphics image object this image was created from, if applicable.

var pixelBuffer: CVPixelBuffer?

The CoreVideo pixel buffer this image was created from, if applicable.

var portraitEffectsMatte: AVPortraitEffectsMatte?

AVPortraitEffectsMatte representation of portrait effects.

var semanticSegmentationMatte: AVSemanticSegmentationMatte?

