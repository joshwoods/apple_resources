

- Core Image
- CIImageProcessorKernel
-  outputFormat 

Type Property

# outputFormat

The processor's output pixel format.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class var outputFormat: CIFormat { get }
```

## Discussion

Override this class property if you want your processor's output to be in a specific CIFormat: BGRA8, RGBAh, RGBAf, or R8. If the `outputFormat` is 0, then the output will be a supported format that best matches the rendering context's workingFormat.

If a processor returns data in a colorspace other than the context working space, then call matchedToWorkingSpace(from:) on the processor output.

If a processor returns data as alpha-unpremultiplied RGBA data, then call premultiplyingAlpha() on the processor output.

