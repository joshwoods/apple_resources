

- AppKit
- NSImage
- NSImage.LoadStatus
-  NSImage.LoadStatus.cancelled 

Case

# NSImage.LoadStatus.cancelled

Image loading was canceled.

macOS

``` source
case cancelled
```

## Discussion

The image contains the portions of the data that have already been successfully decompressed, if any.

## See Also

### Load Status Values

case completed

Enough data is available to completely decompress the image.

case invalidData

An error occurred during image decompression.

case unexpectedEOF

Not enough data was available to fully decompress the image.

case readError

Not enough data was available for full decompression of the image.

