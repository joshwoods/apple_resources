

- Core Image
- CIContext
- CIContextOption
-  workingColorSpace 

Type Property

# workingColorSpace

A key for the color space to use for image operations.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
static let workingColorSpace: CIContextOption
```

## Discussion

By default, Core Image assumes that processing nodes are 128 bits-per-pixel, linear light, premultiplied RGBA floating-point values that use the GenericRGB color space. You can specify a different working color space by providing a Quartz 2D CGColorSpace object (CGColorSpace). Note that the working color space must be RGB based. If you have YUV data as input (or other data that is not RGB based), you can use ColorSync functions to convert to the working color space. (See Quartz 2D Programming Guide for information on creating and using CGColorSpace objects.)

To request that Core Image perform no color management, specify the NSNull object as the value for this key. Use this option for images that don’t contain color data (such as elevation maps, normal vector maps, and sampled function tables).

