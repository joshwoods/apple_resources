

- Image I/O
-  CGImageMetadataTagGetType(\_:) 

Function

# CGImageMetadataTagGetType(\_:)

Returns the type of the metadata tag’s value.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageMetadataTagGetType(_ tag: CGImageMetadataTag) -> CGImageMetadataType
```

## Parameters 

`tag`  

The metadata tag from which to fetch the namespace information.

## Return Value

A constant that indicates the type of the value. For a list of possible return values, see CGImageMetadataType.

## Discussion

To get the value itself, call CGImageMetadataTagCopyValue(_:). Metadata tags store string, number, and Boolean values using the CGImageMetadataType.string type.

## See Also

### Getting the Tag Type

enum CGImageMetadataType

Constants that indicate the XMP type for a metadata tag.

