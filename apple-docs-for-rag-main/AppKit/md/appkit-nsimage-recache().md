

- AppKit
- NSImage
-  recache() 

Instance Method

# recache()

Invalidates and frees offscreen caches of all image representations.

macOS

``` source
func recache()
```

## Discussion

If you modify an image representation, you must send a recache() message to the corresponding image object to force the changes to be recached. The next time any image representation is drawn, it is asked to recreate its cached image. If you do not send this message, the image representation may use the old cache data. This method simply clears the cached image data; it does not delete the `NSCachedImageRep` objects associated with any image representations.

If you do not plan to use an image again right away, you can free its caches to reduce the amount of memory consumed by your program.

## See Also

### Managing Caching Options

var cacheMode: NSImage.CacheMode

The image’s caching mode.

enum CacheMode

Constants that specify the caching policy on a per-image basis.

