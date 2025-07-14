

- Core Image
- CIContext
-  CIImageRepresentationOption 

Structure

# CIImageRepresentationOption

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
struct CIImageRepresentationOption
```

## Topics

### Initializers

init(rawValue: String)

### Type Properties

static let avDepthData: CIImageRepresentationOption

`options` dictionary key for image export methods to represent data as AVDepthData.

static let avPortraitEffectsMatte: CIImageRepresentationOption

static let avSemanticSegmentationMattes: CIImageRepresentationOption

static let depthImage: CIImageRepresentationOption

`options` dictionary key for image export methods to output depth data.

static let disparityImage: CIImageRepresentationOption

`options` dictionary key for image export methods to output disparity data.

static let portraitEffectsMatteImage: CIImageRepresentationOption

static let semanticSegmentationGlassesMatteImage: CIImageRepresentationOption

static let semanticSegmentationHairMatteImage: CIImageRepresentationOption

static let semanticSegmentationSkinMatteImage: CIImageRepresentationOption

static let semanticSegmentationSkyMatteImage: CIImageRepresentationOption

static let semanticSegmentationTeethMatteImage: CIImageRepresentationOption

static let hdrGainMapImage: CIImageRepresentationOption

static let hdrImage: CIImageRepresentationOption

## Relationships

### Conforms To

- Hashable
- RawRepresentable
- Sendable

## See Also

### Rendering Images for Data or File Export

func tiffRepresentation(of: CIImage, format: CIFormat, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any]) -> Data?

Renders the image and exports the resulting image data in TIFF format.

func jpegRepresentation(of: CIImage, colorSpace: CGColorSpace, options: [CIImageRepresentationOption : Any]) -> Data?

Renders the image and exports the resulting image data in JPEG format.

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

