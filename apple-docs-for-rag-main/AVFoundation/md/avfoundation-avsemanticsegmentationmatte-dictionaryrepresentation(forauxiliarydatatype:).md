

- AVFoundation
- AVSemanticSegmentationMatte
-  dictionaryRepresentation(forAuxiliaryDataType:) 

Instance Method

# dictionaryRepresentation(forAuxiliaryDataType:)

Returns a dictionary of primitive map information to use when writing an image file with a semantic segmentation matte.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func dictionaryRepresentation(forAuxiliaryDataType outAuxDataType: AutoreleasingUnsafeMutablePointer?) -> [AnyHashable : Any]?
```

## Parameters 

`outAuxDataType`  

On output, the auxiliary data type to be used when calling the ImageIO framework’s CGImageDestinationAddAuxiliaryDataInfo(_:_:_:) function. Currently supported auxiliary data types are enumerated in `CGImageProperties`.

## Return Value

A dictionary of `CGImageDestination`-compatible semantic segmentation matte information, or `nil` if the auxiliary data type is unsupported.

## See Also

### Creating a Segmentation Matte

convenience init(fromImageSourceAuxiliaryDataType: CFString, dictionaryRepresentation: [AnyHashable : Any]) throws

Returns a new semantic segmentation matte instance from auxiliary image information in an image file.

func replacingSemanticSegmentationMatte(with: CVPixelBuffer) throws -> Self

Returns a semantic segmentation matte instance that wraps the replacement pixel buffer.

func applyingExifOrientation(CGImagePropertyOrientation) -> Self

Returns a new semantic segmentation matte instance with the specified Exif orientation applied.

