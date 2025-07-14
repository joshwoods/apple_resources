

- Latent Semantic Mapping
- LSMMap
-  Map Flags 

API Collection

# Map Flags

Options for creating a map.

## Overview

Specify these options for LSMMapCreate(_:_:). These options can improve mapping accuracy, but may result in a potentially significant increase in memory use.

## Topics

### Constants

var kLSMMapPairs: Int

An option that specifies to use pairs in addition to single words.

var kLSMMapTriplets: Int

An option that specifies to use triplets and pairs in addition to single words.

var kLSMMapHashText: Int

An option that specifies to transform the text so it’s not human-readable.

## See Also

### Creating a Map

func LSMMapCreate(CFAllocator?, CFOptionFlags) -> Unmanaged&lt;LSMMap>

Creates a new Latent Semantic Mapping map.

