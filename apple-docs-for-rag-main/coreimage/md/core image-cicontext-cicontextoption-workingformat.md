

- Core Image
- CIContext
- CIContextOption
-  workingFormat 

Type Property

# workingFormat

An option for the color format to use for intermediate results when rendering with the context.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
static let workingFormat: CIContextOption
```

## Discussion

The value for this key is an NSNumber object containing a CIFormat value. The default working format is RGBA8 for CPU rendering and RGBAf for GPU rendering. For greater color precision, GPU rendering also supports the RGBAh format, but this format requires twice as much memory and can be used only with color management enabled.

