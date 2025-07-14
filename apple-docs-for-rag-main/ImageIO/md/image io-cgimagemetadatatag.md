

- Image I/O
-  CGImageMetadataTag 

Class

# CGImageMetadataTag

An immutable type that contains information about a single piece of image metadata.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class CGImageMetadataTag
```

## Overview

Each CGImageMetadataTag opaque type contains a single EXIF, IPTC, or XMP property. The namespace, prefix, name, type, and value of the tag identify different portions of the tag’s content. For example, the namespace specifies whether the tag is part of the EXIF metadata or a different set of metadata.

You retrieve existing metadata tags from an CGImageMetadata opaque type. You may also create new tags and add them to a CGMutableImageMetadata type, before you assign the updated metadata to an image.

## Topics

### Creating a Metadata Tag

func CGImageMetadataTagCreate(CFString, CFString?, CFString, CGImageMetadataType, CFTypeRef) -> CGImageMetadataTag?

Creates a new image metadata tag, and fills it with the specified information.

### Getting the Attributes of the Tag

func CGImageMetadataTagCopyNamespace(CGImageMetadataTag) -> CFString?

Returns an immutable copy of the tag’s XMP namespace.

func CGImageMetadataTagCopyPrefix(CGImageMetadataTag) -> CFString?

Returns an immutable copy of the tag’s prefix.

func CGImageMetadataTagCopyName(CGImageMetadataTag) -> CFString?

Returns an immutable copy of the tag’s name.

func CGImageMetadataTagCopyValue(CGImageMetadataTag) -> CFTypeRef?

Returns a shallow copy of the tag’s value, which is suitable only for reading.

func CGImageMetadataTagCopyQualifiers(CGImageMetadataTag) -> CFArray?

Returns a shallow copy of the metadata tags that act as qualifiers for the current tag.

### Getting the Tag Type

func CGImageMetadataTagGetType(CGImageMetadataTag) -> CGImageMetadataType

Returns the type of the metadata tag’s value.

enum CGImageMetadataType

Constants that indicate the XMP type for a metadata tag.

### Getting the Core Foundation Type

func CGImageMetadataTagGetTypeID() -> CFTypeID

Returns the type identifier for the image metadata tag opaque type

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### XMP Metadata

class CGImageMetadata

An immutable object that contains the XMP metadata associated with an image.

class CGMutableImageMetadata

An opaque type for adding or modifying image metadata.

XMP Namespaces and Prefixes

Discover the public namespaces and prefixes that exist in XMP metadata tags.

let kCFErrorDomainCGImageMetadata: CFString

The domain for metadata-related errors that originate in the Image I/O framework.

enum CGImageMetadataErrors

Constants for errors that occur when getting or setting metadata information.

