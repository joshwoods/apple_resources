

- Core Image
- CIContext
- CIContextOption
-  outputColorSpace 

Type Property

# outputColorSpace

A key for the color space to use for images before they are rendered to the context.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
static let outputColorSpace: CIContextOption
```

## Discussion

By default, Core Image uses the GenericRGB color space, which leaves color matching to the system. You can specify a different output color space by providing a Quartz 2D CGColorSpace object. (See Quartz 2D Programming Guide for information on creating and using `CGColorSpace` objects.)

To request that Core Image perform no color management, specify the NSNull object as the value for this key. Use this option for images that don’t contain color data (such as elevation maps, normal vector maps, and sampled function tables).

