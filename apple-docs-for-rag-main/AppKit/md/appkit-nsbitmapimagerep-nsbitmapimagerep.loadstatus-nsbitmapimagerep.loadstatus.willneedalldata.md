

- AppKit
- NSBitmapImageRep
- NSBitmapImageRep.LoadStatus
-  NSBitmapImageRep.LoadStatus.willNeedAllData 

Case

# NSBitmapImageRep.LoadStatus.willNeedAllData

Incremental loading cannot be supported.

macOS

``` source
case willNeedAllData
```

## Discussion

Until you call incrementalLoad(from:complete:) with true, this status will be returned. You can continue to call the method but no decompression will take place. Once you do call the method with true, then the image will be decompressed and one of the final three status messages will be returned.

## See Also

### Constants

case unknownType

Not enough data to determine image format. You should continue to provide more data.

case readingHeader

The image format is known, but not enough data has been read to determine the size, depth, etc., of the image. You should continue to provide more data.

case invalidData

An error occurred during image decompression. The image contains the portions of the data that have already been successfully decompressed, if any

case unexpectedEOF

incrementalLoad(from:complete:) was called with true, but not enough data was available for decompression. The image contains the portions of the data that have already been successfully decompressed, if any.

case completed

Enough data has been provided to successfully decompress the image (regardless of the complete: flag).

