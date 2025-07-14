

- AppKit
- NSImage
-  cacheMode 

Instance Property

# cacheMode

The image’s caching mode.

macOS

``` source
var cacheMode: NSImage.CacheMode { get set }
```

## Discussion

The caching mode determines when the image representations use offscreen caches. Offscreen caches speed up rendering time but do so by using extra memory. In the default caching mode (`NSImageCacheDefault`), each image representation chooses the caching technique that produces the fastest drawing times. For example, in the default mode, the `NSPDFImageRep` and `NSEPSImageRep` classes use the `NSImageCacheAlways` mode but the `NSBitmapImageRep` class uses the `NSImageCacheBySize` mode. For a list of possible values, see NSImage.CacheMode. This value is set to `NSImageCacheDefault` by default.

For more information on image caching behavior, see the Images chapter of Cocoa Drawing Guide.

## See Also

### Managing Caching Options

func recache()

Invalidates and frees offscreen caches of all image representations.

enum CacheMode

Constants that specify the caching policy on a per-image basis.

