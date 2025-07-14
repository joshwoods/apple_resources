

- Image I/O
-  CGImageMetadataCopyTagMatchingImageProperty(\_:\_:\_:) 

Function

# CGImageMetadataCopyTagMatchingImageProperty(\_:\_:\_:)

Searches for the specified image property and, if found, returns the corresponding tag object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageMetadataCopyTagMatchingImageProperty(
    _ metadata: CGImageMetadata,
    _ dictionaryName: CFString,
    _ propertyName: CFString
) -> CGImageMetadataTag?
```

## Parameters 

`metadata`  

The metadata object to search.

`dictionaryName`  

The metadata subdictionary to which the image property belongs. For example, specify kCGImagePropertyExifDictionary for image properties that are part of the image’s EXIF metadata.

`propertyName`  

The name of the property. For example, specify kCGImagePropertyTIFFOrientation, kCGImagePropertyExifDateTimeOriginal, or kCGImagePropertyIPTCKeywords. If the specified property is unsupported by the metadata object, this function logs a warning.

## Return Value

The CGImageMetadataTag object that corresponds to the specified property, or `NULL` if the property wasn’t found.

## Discussion

Use this function to quickly search the different metadata dictionaries for a specific tag. The returned tag object contains appropriate values for all fields, including the namespace, prefix, and XMP type.

When you request an EXIF or IPTC property, this function fills in the namespace, prefix, and XMP type information by copying information from an appropriate XMP type. For example, when you request the kCGImagePropertyExifDateTimeOriginal property, the function fills in the information using the `photoshop:DateTime` XMP tag. When this bridging occurs, property fields retain their XMP format, rather than the EXIF or IPTC format.

## See Also

### Getting the Metadata Tags

func CGImageMetadataCopyTagWithPath(CGImageMetadata, CGImageMetadataTag?, CFString) -> CGImageMetadataTag?

Searches for a specific metadata tag within a metadata collection.

func CGImageMetadataCopyTags(CGImageMetadata) -> CFArray?

Returns an array of root-level metadata tags from the specified metadata object.

func CGImageMetadataCopyStringValueWithPath(CGImageMetadata, CGImageMetadataTag?, CFString) -> CFString?

Searches the metadata for the specified tag, and returns its string value if it exists.

