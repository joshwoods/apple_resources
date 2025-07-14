

- AVFoundation
-  AVSemanticSegmentationMatte 

Class

# AVSemanticSegmentationMatte

An object that wraps a matting image for a particular semantic segmentation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class AVSemanticSegmentationMatte
```

## Overview

The matting image stores its pixel data as CVPixelBuffer objects in kCVPixelFormatType_OneComponent8 format. The image file contains the semantic segmentation matte as an auxiliary image, accessible using the ImageIO framework’s CGImageSourceCopyAuxiliaryDataInfoAtIndex(_:_:_:) function.

## Topics

### Creating a Segmentation Matte

convenience init(fromImageSourceAuxiliaryDataType: CFString, dictionaryRepresentation: [AnyHashable : Any]) throws

Returns a new semantic segmentation matte instance from auxiliary image information in an image file.

func replacingSemanticSegmentationMatte(with: CVPixelBuffer) throws -> Self

Returns a semantic segmentation matte instance that wraps the replacement pixel buffer.

func applyingExifOrientation(CGImagePropertyOrientation) -> Self

Returns a new semantic segmentation matte instance with the specified Exif orientation applied.

func dictionaryRepresentation(forAuxiliaryDataType: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> [AnyHashable : Any]?

Returns a dictionary of primitive map information to use when writing an image file with a semantic segmentation matte.

### Inspecting a Segmentation Matte

var matteType: AVSemanticSegmentationMatte.MatteType

The semantic segmentation matte image type.

struct MatteType

A structure that defines the types of segmentation matte images that you can capture along with the primary image.

var mattingImage: CVPixelBuffer

The semantic segmentation matte’s internal image.

var pixelFormatType: OSType

The pixel format type for this object’s internal matting image.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Matte data

class AVPortraitEffectsMatte

An auxiliary image used to separate foreground from background with high resolution.

