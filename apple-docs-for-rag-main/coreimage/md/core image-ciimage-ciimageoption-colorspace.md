

- Core Image
- CIImage
- CIImageOption
-  colorSpace 

Type Property

# colorSpace

The key for a color space.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
static let colorSpace: CIImageOption
```

## Discussion

For more information on this data type see `CGColorSpace`. Typically you use this option when you need to load an elevation, mask, normal vector, or RAW sensor data directly from a file without color correcting it. This constant specifies to override Core Image, which, by default, assumes that data is in GenericRGB.

The value you supply for this dictionary key must be a CGColorSpace data type. If a value for this key isn’t supplied, the image’s colorSpace dictionary are populated automatically by calling CGImageSourceCopyPropertiesAtIndex(_:_:_:). To request that Core Image perform no color management, specify the NSNull object as the value for this key. Use this option for images that don’t contain color data (such as elevation maps, normal vector maps, and sampled function tables).

