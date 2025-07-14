

- AVFoundation
- AVSemanticSegmentationMatte
-  applyingExifOrientation(\_:) 

Instance Method

# applyingExifOrientation(\_:)

Returns a new semantic segmentation matte instance with the specified Exif orientation applied.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func applyingExifOrientation(_ exifOrientation: CGImagePropertyOrientation) -> Self
```

## Parameters 

`exifOrientation`  

A CGImagePropertyOrientation value expressing how the matte should be rotated or mirrored.

## Return Value

A new semantic segmentation matte instance.

## Discussion

This method throws an invalidArgumentException if you pass an unrecognized `exifOrientation`.

## See Also

### Creating a Segmentation Matte

convenience init(fromImageSourceAuxiliaryDataType: CFString, dictionaryRepresentation: [AnyHashable : Any]) throws

Returns a new semantic segmentation matte instance from auxiliary image information in an image file.

func replacingSemanticSegmentationMatte(with: CVPixelBuffer) throws -> Self

Returns a semantic segmentation matte instance that wraps the replacement pixel buffer.

func dictionaryRepresentation(forAuxiliaryDataType: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> [AnyHashable : Any]?

Returns a dictionary of primitive map information to use when writing an image file with a semantic segmentation matte.

