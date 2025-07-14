

- AVFoundation
- AVSemanticSegmentationMatte
-  AVSemanticSegmentationMatte.MatteType 

Structure

# AVSemanticSegmentationMatte.MatteType

A structure that defines the types of segmentation matte images that you can capture along with the primary image.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MatteType
```

## Topics

### Matte Types

static let hair: AVSemanticSegmentationMatte.MatteType

A matting image that segments the hair from all people in the visible field of view of an image.

static let skin: AVSemanticSegmentationMatte.MatteType

A matting image that segments the skin from all people in the visible field of view of an image.

static let teeth: AVSemanticSegmentationMatte.MatteType

A matting image that segments the teeth from all people in the visible field of view of an image.

static let glasses: AVSemanticSegmentationMatte.MatteType

A matting image that segments eyeglasses and sunglasses from all people in the visible field of view of an image.

### Initializers

init(rawValue: String)

Creates a matte type with a string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting a Segmentation Matte

var matteType: AVSemanticSegmentationMatte.MatteType

The semantic segmentation matte image type.

var mattingImage: CVPixelBuffer

The semantic segmentation matte’s internal image.

var pixelFormatType: OSType

The pixel format type for this object’s internal matting image.

