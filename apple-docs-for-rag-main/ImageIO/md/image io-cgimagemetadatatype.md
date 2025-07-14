

- Image I/O
-  CGImageMetadataType 

Enumeration

# CGImageMetadataType

Constants that indicate the XMP type for a metadata tag.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum CGImageMetadataType
```

## Overview

Use these constants to identify the type of metadata in a CGImageMetadataTag opaque type. The type tells you how to interpret the value of the metadata tag. When creating a new CGImageMetadataTag, specify a type so the system knows how to serialize the data to the XMP format.

## Topics

### Metadata Types

case invalid

An invalid metadata type.

case `default`

The default type for new tags.

case string

A string value.

case arrayUnordered

An array that doesn’t preserve the order of items.

case arrayOrdered

An array that preserves the order of items.

case alternateArray

An ordered array, in which all elements are alternates for the same value.

case alternateText

An alternate array, in which all elements are localized strings for the same value.

case structure

A collection of keys and values.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Tag Type

func CGImageMetadataTagGetType(CGImageMetadataTag) -> CGImageMetadataType

Returns the type of the metadata tag’s value.

