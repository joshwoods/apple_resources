

- Core Image
- CIFilter
- Stylizing Filters
- CIShadedMaterial
-  shadingImage 

Instance Property

# shadingImage

The image to use as the height field.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var shadingImage: CIImage? { get set }
```

**Required**

## Discussion

The resulting image has greater heights with lighter shades, and lesser heights (lower areas) with darker shades.

