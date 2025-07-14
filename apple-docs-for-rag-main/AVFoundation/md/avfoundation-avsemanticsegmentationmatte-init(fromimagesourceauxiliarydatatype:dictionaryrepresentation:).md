

- AVFoundation
- AVSemanticSegmentationMatte
-  init(fromImageSourceAuxiliaryDataType:dictionaryRepresentation:) 

Initializer

# init(fromImageSourceAuxiliaryDataType:dictionaryRepresentation:)

Returns a new semantic segmentation matte instance from auxiliary image information in an image file.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
convenience init(
    fromImageSourceAuxiliaryDataType imageSourceAuxiliaryDataType: CFString,
    dictionaryRepresentation imageSourceAuxiliaryDataInfoDictionary: [AnyHashable : Any]
) throws
```

## Parameters 

`imageSourceAuxiliaryDataType`  

The `kCGImageAuxiliaryDataType` constants corresponding to the semantic segmentation matte being created (see `CGImageProperties`).

`imageSourceAuxiliaryDataInfoDictionary`  

A dictionary of primitive semantic segmentation matte information obtained from CGImageSourceCopyAuxiliaryDataInfoAtIndex(_:_:_:).

## Return Value

A new semantic segmentation matte instance, or `nil` if the auxiliary data info dictionary is malformed.

## See Also

### Creating a Segmentation Matte

func replacingSemanticSegmentationMatte(with: CVPixelBuffer) throws -> Self

Returns a semantic segmentation matte instance that wraps the replacement pixel buffer.

func applyingExifOrientation(CGImagePropertyOrientation) -> Self

Returns a new semantic segmentation matte instance with the specified Exif orientation applied.

func dictionaryRepresentation(forAuxiliaryDataType: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> [AnyHashable : Any]?

Returns a dictionary of primitive map information to use when writing an image file with a semantic segmentation matte.

