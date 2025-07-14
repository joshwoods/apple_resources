

- Image I/O
-  CGImageMetadataSetValueMatchingImageProperty(\_:\_:\_:\_:) 

Function

# CGImageMetadataSetValueMatchingImageProperty(\_:\_:\_:\_:)

Updates the value of the metadata tag assigned to the specified image property.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageMetadataSetValueMatchingImageProperty(
    _ metadata: CGMutableImageMetadata,
    _ dictionaryName: CFString,
    _ propertyName: CFString,
    _ value: CFTypeRef
) -> Bool
```

## Parameters 

`metadata`  

The metadata object that contains the tag.

`dictionaryName`  

The metadata subdictionary to which the image property belongs. For example, specify kCGImagePropertyExifDictionary for image properties that are part of the image’s EXIF metadata. This function doesn’t support all dictionaries.

`propertyName`  

The name of the property. For example, specify kCGImagePropertyTIFFOrientation, kCGImagePropertyExifDateTimeOriginal, or kCGImagePropertyIPTCKeywords. If the specified property is unsupported by the metadata object, this function logs a warning.

`value`  

The new value for the property. The new value’s type must match the XMP type of the metadata tag.

## Return Value

`true` if this function set the tag successfully, or `false` if a problem occurred.

## Discussion

Use this function to update the value of a property in the specified metadata collection. If you try to set the value of an EXIF or IPTC property, this function matches it to an appropriate XMP tag. For example, when you set the value of the kCGImagePropertyExifDateTimeOriginal property, this function sets the value of the `photoshop:DateTime` XMP tag.

If the metdata object doesn’t contain the tag, this function creates it and populates it with appropriate XMP information.

## See Also

### Setting the Values of Tags

func CGImageMetadataSetValueWithPath(CGMutableImageMetadata, CGImageMetadataTag?, CFString, CFTypeRef) -> Bool

Update the value of an existing metadata tag, or create a new tag using the specified information.

func CGImageMetadataSetTagWithPath(CGMutableImageMetadata, CGImageMetadataTag?, CFString, CGImageMetadataTag) -> Bool

Sets the tag at the specified path in the metadata object.

func CGImageMetadataRemoveTagWithPath(CGMutableImageMetadata, CGImageMetadataTag?, CFString) -> Bool

Removes the tag at the specified path from the metadata object.

