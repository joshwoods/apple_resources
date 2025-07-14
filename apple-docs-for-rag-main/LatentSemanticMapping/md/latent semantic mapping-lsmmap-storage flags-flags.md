

- Latent Semantic Mapping
- LSMMap
-  Storage Flags 

API Collection

# Storage Flags

Options for loading and saving a map to a file.

## Overview

Specify these options for LSMMapCreateFromURL(_:_:_:) and LSMMapWriteToURL(_:_:_:).

## Topics

### Constants

var kLSMMapDiscardCounts: Int

An option that specifies not to keep counts.

var kLSMMapLoadMutable: Int

An option that specifies to load the map as mutable in training state.

var kLSMMapHashText: Int

An option that specifies to transform the text so it’s not human-readable.

## See Also

### Loading and Saving a Map

func LSMMapCreateFromURL(CFAllocator?, CFURL, CFOptionFlags) -> Unmanaged&lt;LSMMap>?

Loads a map from the specified file.

func LSMMapWriteToURL(LSMMap, CFURL, CFOptionFlags) -> OSStatus

Compiles the map, if necessary, and stores it into the specified file.

func LSMMapWriteToStream(LSMMap, LSMText?, CFWriteStream, CFOptionFlags) -> OSStatus

Writes information about a map or text to a stream in text form.

