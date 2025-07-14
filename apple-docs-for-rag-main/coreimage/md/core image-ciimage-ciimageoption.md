

- Core Image
- CIImage
-  CIImageOption 

Structure

# CIImageOption

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
struct CIImageOption
```

## Topics

### Initializers

init(rawValue: String)

### Type Properties

static let applyOrientationProperty: CIImageOption

The key for transforming an image according to orientation metadata.

static let auxiliaryDepth: CIImageOption

The key into the properties dictionary indicating whether to return an auxiliary depth image.

static let auxiliaryDisparity: CIImageOption

The key into the properties dictionary indicating whether to return an auxiliary disparity image.

static let auxiliaryHDRGainMap: CIImageOption

static let auxiliaryPortraitEffectsMatte: CIImageOption

The key into the properties dictionary indicating whether to return auxiliary portrait effects matte.

static let auxiliarySemanticSegmentationGlassesMatte: CIImageOption

static let auxiliarySemanticSegmentationHairMatte: CIImageOption

static let auxiliarySemanticSegmentationSkinMatte: CIImageOption

static let auxiliarySemanticSegmentationSkyMatte: CIImageOption

static let auxiliarySemanticSegmentationTeethMatte: CIImageOption

static let cacheImmediately: CIImageOption

static let colorSpace: CIImageOption

The key for a color space.

static let expandToHDR: CIImageOption

A Boolean value that indicates whether to read Gain Map HDR images as HDR.

static let nearestSampling: CIImageOption

The key into the properties dictionary to indicate whether to use nearest-neighbor sampling.

static let properties: CIImageOption

The key for image metadata properties.

static let providerTileSize: CIImageOption

A key for the image tiles size. The associated value is an `NSArray` that contains`NSNumber` objects for the dimensions of the image tiles requested from the image provider.

static let providerUserInfo: CIImageOption

A key for data needed by the image provider. The associated value is an object that contains the needed data.

static let textureFormat: CIImageOption

The key for an OpenGL texture format.

Deprecated

static let textureTarget: CIImageOption

The key for an OpenGL texture target.

Deprecated

static let toneMapHDRtoSDR: CIImageOption

static let contentHeadroom: CIImageOption

## Relationships

### Conforms To

- Hashable
- RawRepresentable
- Sendable

