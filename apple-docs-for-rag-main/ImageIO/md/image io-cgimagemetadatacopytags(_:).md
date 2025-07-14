

- Image I/O
-  CGImageMetadataCopyTags(\_:) 

Function

# CGImageMetadataCopyTags(\_:)

Returns an array of root-level metadata tags from the specified metadata object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageMetadataCopyTags(_ metadata: CGImageMetadata) -> CFArray?
```

## Parameters 

`metadata`  

The metadata object that contains the tags.

## Return Value

An array that contains a shallow copy of all root-level CGImageMetadataTag objects. This array contains only the root-level tags. It doesn’t contain any nested tags.

## See Also

### Getting the Metadata Tags

func CGImageMetadataCopyTagWithPath(CGImageMetadata, CGImageMetadataTag?, CFString) -> CGImageMetadataTag?

Searches for a specific metadata tag within a metadata collection.

func CGImageMetadataCopyTagMatchingImageProperty(CGImageMetadata, CFString, CFString) -> CGImageMetadataTag?

Searches for the specified image property and, if found, returns the corresponding tag object.

func CGImageMetadataCopyStringValueWithPath(CGImageMetadata, CGImageMetadataTag?, CFString) -> CFString?

Searches the metadata for the specified tag, and returns its string value if it exists.

