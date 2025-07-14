

- Image I/O
-  kCGImageMetadataEnumerateRecursively 

Global Variable

# kCGImageMetadataEnumerateRecursively

An option to enumerate recursively through a set of metadata tags.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCGImageMetadataEnumerateRecursively: CFString
```

## Discussion

The value of this key is a CFBoolean. Set the value to kOSBooleanTrue to enumerate all tags recursively. Set the value to kCFBooleanFalse to enumerate only the direct children of the root path you specify.

When you call CGImageMetadataEnumerateTagsUsingBlock(_:_:_:_:), include this option if you want the enumeration behavior to search recursively through the available tags. If you don’t specify this key, the function behaves as if the value is false.

## See Also

### Enumerating the Metadata Tags

func CGImageMetadataEnumerateTagsUsingBlock(CGImageMetadata, CFString?, CFDictionary?, CGImageMetadataTagBlock)

Enumerates the tags of a metadata object and executes the specified block on each tag.

typealias CGImageMetadataTagBlock

The block to execute when enumerating the tags of a metadata object.

