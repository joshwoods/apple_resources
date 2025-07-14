

- AppKit
- NSImage
- NSImage.CacheMode
-  NSImage.CacheMode.default 

Case

# NSImage.CacheMode.default

Caching is unspecified.

macOS

``` source
case `default`
```

## Discussion

Use the image rep’s default.

## See Also

### Cache Options

case always

Always generate a cache when drawing.

case bySize

Cache if the cache size is smaller than the original data.

case never

Never cache; always draw direct.

