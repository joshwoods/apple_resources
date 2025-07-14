

- AppKit
- NSImage
-  NSImage.CacheMode 

Enumeration

# NSImage.CacheMode

Constants that specify the caching policy on a per-image basis.

macOS

``` source
enum CacheMode
```

## Overview

Set the caching policy using the cacheMode property.

The following table specifies the default caching policy for the various types of image representation.

| Image Rep Class | Default caching policy |
|----|----|
| `NSBitmapImageRep` | `NSImageCacheBySize`. Cache if bitmap is 32-bits in 16-bit world or greater than 72 dpi. |
| `NSPICTImageRep` | `NSImageCacheBySize`. Same reasoning as `NSBitmapImageRep` in the event the PICT contains a bitmap. |
| `NSPDFImageRep` | `NSImageCacheAlways` |
| `NSCIImageRep` | `NSImageCacheBySize`. Cache if the bitmap depth does not match the screen depth or the resolution is greater than 72 dpi. |
| `NSEPSImageRep` | `NSImageCacheAlways` |
| `NSCustomImageRep` | `NSImageCacheAlways` |

## Topics

### Cache Options

case `default`

Caching is unspecified.

case always

Always generate a cache when drawing.

case bySize

Cache if the cache size is smaller than the original data.

case never

Never cache; always draw direct.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Caching Options

var cacheMode: NSImage.CacheMode

The image’s caching mode.

func recache()

Invalidates and frees offscreen caches of all image representations.

