

- Image I/O
- CGImageMetadataType
-  CGImageMetadataType.arrayOrdered 

Case

# CGImageMetadataType.arrayOrdered

An array that preserves the order of items.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case arrayOrdered
```

## Discussion

During serialization, this type becomes `` in the XMP format.

## See Also

### Metadata Types

case invalid

An invalid metadata type.

case `default`

The default type for new tags.

case string

A string value.

case arrayUnordered

An array that doesn’t preserve the order of items.

case alternateArray

An ordered array, in which all elements are alternates for the same value.

case alternateText

An alternate array, in which all elements are localized strings for the same value.

case structure

A collection of keys and values.

