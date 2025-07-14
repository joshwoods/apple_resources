

- Image I/O
-  CGImageMetadataTagCopyValue(\_:) 

Function

# CGImageMetadataTagCopyValue(\_:)

Returns a shallow copy of the tag’s value, which is suitable only for reading.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageMetadataTagCopyValue(_ tag: CGImageMetadataTag) -> CFTypeRef?
```

## Parameters 

`tag`  

The metadata tag from which to fetch the namespace information.

## Return Value

A copy of the tag’s value. Possible return types are CFString, CFNumber, CFBoolean, CFArray, and CFDictionary.

## Discussion

Use this method to obtain the value when you want to use or display that value elsewhere. Any changes you make to the returned value don’t change the contents of the metadata tag. To change the value, call CGImageMetadataSetValueWithPath(_:_:_:_:) or CGImageMetadataSetTagWithPath(_:_:_:_:) instead.

## See Also

### Getting the Attributes of the Tag

func CGImageMetadataTagCopyNamespace(CGImageMetadataTag) -> CFString?

Returns an immutable copy of the tag’s XMP namespace.

func CGImageMetadataTagCopyPrefix(CGImageMetadataTag) -> CFString?

Returns an immutable copy of the tag’s prefix.

func CGImageMetadataTagCopyName(CGImageMetadataTag) -> CFString?

Returns an immutable copy of the tag’s name.

func CGImageMetadataTagCopyQualifiers(CGImageMetadataTag) -> CFArray?

Returns a shallow copy of the metadata tags that act as qualifiers for the current tag.

