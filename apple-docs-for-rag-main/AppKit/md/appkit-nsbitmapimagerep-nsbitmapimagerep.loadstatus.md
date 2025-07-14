

- AppKit
- NSBitmapImageRep
-  NSBitmapImageRep.LoadStatus 

Enumeration

# NSBitmapImageRep.LoadStatus

Constants that identify the loading status of the image.

macOS

``` source
enum LoadStatus
```

## Overview

These status values are returned by incrementalLoad(from:complete:).

## Topics

### Constants

case unknownType

Not enough data to determine image format. You should continue to provide more data.

case readingHeader

The image format is known, but not enough data has been read to determine the size, depth, etc., of the image. You should continue to provide more data.

case willNeedAllData

Incremental loading cannot be supported.

case invalidData

An error occurred during image decompression. The image contains the portions of the data that have already been successfully decompressed, if any

case unexpectedEOF

incrementalLoad(from:complete:) was called with true, but not enough data was available for decompression. The image contains the portions of the data that have already been successfully decompressed, if any.

case completed

Enough data has been provided to successfully decompress the image (regardless of the complete: flag).

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Loading Images Incrementally

func incrementalLoad(from: Data, complete: Bool) -> Int

Loads the current image data into an incrementally-loaded image representation and returns the current status of the image.

