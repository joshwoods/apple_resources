

- AppKit
- NSImage
-  NSImage.LoadStatus 

Enumeration

# NSImage.LoadStatus

Status values for incremental image loading.

macOS

``` source
enum LoadStatus
```

## Topics

### Load Status Values

case completed

Enough data is available to completely decompress the image.

case cancelled

Image loading was canceled.

case invalidData

An error occurred during image decompression.

case unexpectedEOF

Not enough data was available to fully decompress the image.

case readError

Not enough data was available for full decompression of the image.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

