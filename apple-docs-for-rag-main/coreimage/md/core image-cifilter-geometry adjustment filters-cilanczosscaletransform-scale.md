

- Core Image
- CIFilter
- Geometry Adjustment Filters
- CILanczosScaleTransform
-  scale 

Instance Property

# scale

The scaling factor to use on the image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var scale: Float { get set }
```

**Required**

## Discussion

Values less than 1.0 scale down the images. Values greater than 1.0 scale up the image.

