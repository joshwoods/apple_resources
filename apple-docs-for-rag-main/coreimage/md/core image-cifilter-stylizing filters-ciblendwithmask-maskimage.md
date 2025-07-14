

- Core Image
- CIFilter
- Stylizing Filters
- CIBlendWithMask
-  maskImage 

Instance Property

# maskImage

A grayscale mask that defines the blend.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var maskImage: CIImage? { get set }
```

**Required**

## Discussion

When a mask value is 0.0, the result is the background. When the mask value is 1.0, the result is the image.

