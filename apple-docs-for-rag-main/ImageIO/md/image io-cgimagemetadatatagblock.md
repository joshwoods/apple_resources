

- Image I/O
-  CGImageMetadataTagBlock 

Type Alias

# CGImageMetadataTagBlock

The block to execute when enumerating the tags of a metadata object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias CGImageMetadataTagBlock = (CFString, CGImageMetadataTag) -> Bool
```

## Parameters 

`path`  

The full path to the tag in the metadata container.

`tag`  

The CGImageMetadataTag object that contains the tag information. Never modify this object from your block. If you want to change the tag, save a reference to it and make your changes later.

## Return Value

`true` to continue enumerating the tags, or `false` to stop.

## See Also

### Enumerating the Metadata Tags

func CGImageMetadataEnumerateTagsUsingBlock(CGImageMetadata, CFString?, CFDictionary?, CGImageMetadataTagBlock)

Enumerates the tags of a metadata object and executes the specified block on each tag.

let kCGImageMetadataEnumerateRecursively: CFString

An option to enumerate recursively through a set of metadata tags.

