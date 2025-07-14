

- Image I/O
-  CGImageMetadataTagCopyName(\_:) 

Function

# CGImageMetadataTagCopyName(\_:)

Returns an immutable copy of the tag’s name.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageMetadataTagCopyName(_ tag: CGImageMetadataTag) -> CFString?
```

## Parameters 

`tag`  

The metadata tag from which to fetch the namespace information.

## Return Value

A string that contains the tag’s name. You are responsible for releasing this string.

## See Also

### Getting the Attributes of the Tag

func CGImageMetadataTagCopyNamespace(CGImageMetadataTag) -> CFString?

Returns an immutable copy of the tag’s XMP namespace.

func CGImageMetadataTagCopyPrefix(CGImageMetadataTag) -> CFString?

Returns an immutable copy of the tag’s prefix.

func CGImageMetadataTagCopyValue(CGImageMetadataTag) -> CFTypeRef?

Returns a shallow copy of the tag’s value, which is suitable only for reading.

func CGImageMetadataTagCopyQualifiers(CGImageMetadataTag) -> CFArray?

Returns a shallow copy of the metadata tags that act as qualifiers for the current tag.

