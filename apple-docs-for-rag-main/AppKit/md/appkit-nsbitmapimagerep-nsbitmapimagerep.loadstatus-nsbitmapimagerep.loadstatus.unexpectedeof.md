

- AppKit
- NSBitmapImageRep
- NSBitmapImageRep.LoadStatus
-  NSBitmapImageRep.LoadStatus.unexpectedEOF 

Case

# NSBitmapImageRep.LoadStatus.unexpectedEOF

incrementalLoad(from:complete:) was called with true, but not enough data was available for decompression. The image contains the portions of the data that have already been successfully decompressed, if any.

macOS

``` source
case unexpectedEOF
```

## See Also

### Constants

case unknownType

Not enough data to determine image format. You should continue to provide more data.

case readingHeader

The image format is known, but not enough data has been read to determine the size, depth, etc., of the image. You should continue to provide more data.

case willNeedAllData

Incremental loading cannot be supported.

case invalidData

An error occurred during image decompression. The image contains the portions of the data that have already been successfully decompressed, if any

case completed

Enough data has been provided to successfully decompress the image (regardless of the complete: flag).

