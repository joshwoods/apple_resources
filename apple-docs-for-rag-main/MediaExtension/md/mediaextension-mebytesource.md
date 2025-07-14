

- MediaExtension
-  MEByteSource 

Class

# MEByteSource

Provides read access to the data in a media asset file.

macOS 14.0+

``` source
class MEByteSource
```

## Overview

Media Toolbox passes an `MEByteSource` instance for the media asset’s primary file when it initializes an MEFormatReader object. The format reader may call byteSourceForRelatedFileName(_:) to request additional byte sources for related files in the same directory as the primary file.

## Topics

### Inspecting a byte source

var fileName: String

The name of the file for the byte source.

var fileLength: Int64

The length of the byte source file.

var contentType: UTType?

The format of the byte source file.

var relatedFileNamesInSameDirectory: [String]

An array of related file names in the parent directory of the byte source file.

### Performing operations on a byte source

func availableLength(at: Int64) -> Int64

Gets the number of available bytes from the offset within the byte source.

func byteSourceForRelatedFileName(String) throws -> MEByteSource

Creates a new byte source for a related file.

func read(length: Int, from: Int64, completionHandler: (Data?, (any Error)?) -> Void)

Reads bytes from a byte source into a data object.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

