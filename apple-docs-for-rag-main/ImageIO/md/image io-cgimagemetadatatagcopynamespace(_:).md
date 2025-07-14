

- Image I/O
-  CGImageMetadataTagCopyNamespace(\_:) 

Function

# CGImageMetadataTagCopyNamespace(\_:)

Returns an immutable copy of the tag’s XMP namespace.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageMetadataTagCopyNamespace(_ tag: CGImageMetadataTag) -> CFString?
```

## Parameters 

`tag`  

The metadata tag from which to fetch the namespace information.

## Return Value

An immutable string that contains the tag’s namespace. For a list of public namespaces, see XMP Namespaces and Prefixes. You are responsible for releasing this string.

## Discussion

By convention, namespaces end with either a `/` or `#` character. For example, EXIF metadata uses the namespace `http://ns.adobe.com/exif/1.0/`. Custom namespaces must be a valid XML namespace.

## See Also

### Getting the Attributes of the Tag

func CGImageMetadataTagCopyPrefix(CGImageMetadataTag) -> CFString?

Returns an immutable copy of the tag’s prefix.

func CGImageMetadataTagCopyName(CGImageMetadataTag) -> CFString?

Returns an immutable copy of the tag’s name.

func CGImageMetadataTagCopyValue(CGImageMetadataTag) -> CFTypeRef?

Returns a shallow copy of the tag’s value, which is suitable only for reading.

func CGImageMetadataTagCopyQualifiers(CGImageMetadataTag) -> CFArray?

Returns a shallow copy of the metadata tags that act as qualifiers for the current tag.

