

- Core Image
- CIContext
-  jpegRepresentation(of:colorSpace:options:) 

Instance Method

# jpegRepresentation(of:colorSpace:options:)

Renders the image and exports the resulting image data in JPEG format.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func jpegRepresentation(
    of image: CIImage,
    colorSpace: CGColorSpace,
    options: [CIImageRepresentationOption : Any] = [:]
) -> Data?
```

## Parameters 

`image`  

The image object to render.

`colorSpace`  

The color space in which to render the output image. This color space must conform to either the CGColorSpaceModel.rgb or CGColorSpaceModel.monochrome model and must be compatible with the specified pixel format.

`options`  

A dictionary with additional options for export. Use the kCGImageDestinationLossyCompressionQuality key to specify JPEG compression level. Other supported keys include avDepthData, depthImage, and disparityImage.

## Return Value

A data representation of the rendered image in JPEG format, or `nil` if the image could not be rendered.

## Discussion

To render an image for export, the image’s contents must not be empty and its extent dimensions must be finite. To export after applying a filter whose output has infinite extent, see the clampedToExtent() method.

## See Also

### Rendering Images for Data or File Export

func tiffRepresentation(of: CIImage, format: CIFormat, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any]) -> Data?

Renders the image and exports the resulting image data in TIFF format.

func pngRepresentation(of: CIImage, format: CIFormat, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any]) -> Data?

Renders the image and exports the resulting image data in PNG format.

func heifRepresentation(of: CIImage, format: CIFormat, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any]) -> Data?

Renders the image and exports the resulting image data in HEIF format.

func heif10Representation(of: CIImage, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any]) -> Data

Renders the image and exports the resulting image data in HEIF10 format.

func openEXRRepresentation(of: CIImage, options: [CIImageRepresentationOption : Any]) -> Data

Renders the image and exports the resulting image data in open EXR format.

func writeTIFFRepresentation(of: CIImage, to: URL, format: CIFormat, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any])

Renders the image and exports the resulting image data as a file in TIFF format.

func writeJPEGRepresentation(of: CIImage, to: URL, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any])

Renders the image and exports the resulting image data as a file in JPEG format.

func writePNGRepresentation(of: CIImage, to: URL, format: CIFormat, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any])

Renders the image and exports the resulting image data as a file in PNG format.

func writeHEIFRepresentation(of: CIImage, to: URL, format: CIFormat, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any])

Renders the image and exports the resulting image data as a file in HEIF format.

func writeHEIF10Representation(of: CIImage, to: URL, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any])

Renders the image and exports the resulting image data as a file in HEIF10 format.

func writeOpenEXRRepresentation(of: CIImage, to: URL, options: [CIImageRepresentationOption : Any])

Renders the image and exports the resulting image data as a file in open EXR format.

struct CIImageRepresentationOption

