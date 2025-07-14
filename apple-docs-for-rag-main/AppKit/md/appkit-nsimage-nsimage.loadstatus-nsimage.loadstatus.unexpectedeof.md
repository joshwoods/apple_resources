

- AppKit
- NSImage
- NSImage.LoadStatus
-  NSImage.LoadStatus.unexpectedEOF 

Case

# NSImage.LoadStatus.unexpectedEOF

Not enough data was available to fully decompress the image.

macOS

``` source
case unexpectedEOF
```

## Discussion

The image contains the portions of the data that have already been successfully decompressed, if any.

## See Also

### Load Status Values

case completed

Enough data is available to completely decompress the image.

case cancelled

Image loading was canceled.

case invalidData

An error occurred during image decompression.

case readError

Not enough data was available for full decompression of the image.

